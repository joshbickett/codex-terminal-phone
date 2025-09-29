# Running Codex in a Terminal From Your Phone

I love Codex CLI. Recently, I wondered if I could run it from my phone. There is ChatGPT iOS Codex, but that comes with limitations. If I run Codex CLI in a terminal from my phone, I can do **anything**. For example, I built the initial version of this repo entirely from my phone in the terminal with Codex. I asked Codex to create the markdown file and add the steps, then I described the steps as you'll see below. I also recorded this Codex prompt so you can watch it. I SFTPed it from my phone to the Codex terminal and then asked Codex to speed up the recording 6×. Finally, I pushed it up so you could see the demo below!

## Workflow Demo (6× speed)

<p align="center">
  <img src="ScreenRecording_09-28-2025_21-14-54_1_speed6.gif" alt="Codex Terminal Phone workflow demo (6× speed)" width="240">
</p>


## Setup Steps

<ol>
  <li>
    <p>Launch a free GCP <code>e2-micro</code> Compute Engine VM and grab its external IP.</p>
    <p align="center">
      <img src="gcp.png" alt="Creating an e2-micro VM in GCP" width="300">
    </p>
  </li>
  <li>
    <p>Install Termius on iOS and sign in with your Termius account.</p>
  </li>
  <li>
    <p>Generate an SSH key pair in Termius (<code>Keychain</code> → <code>+</code> → <code>New Key</code> → <code>ED25519</code>) to create an <code>ssh-ed25519</code> key, then copy the public key.</p>
  </li>
  <li>
    <p>In the Google Cloud console, open your VM, click <code>Edit</code>, add the Termius public key under <code>SSH Keys</code>, and save.</p>
  </li>
  <li>
    <p>Add the VM as a host in Termius, reuse the username from your key, paste the external IP, and attach the saved key.</p>
    <p align="center">
      <img src="termius.png" alt="Configuring the VM host in Termius" width="420">
    </p>
  </li>
  <li>
    <p>Open the new host in Termius to SSH into the GCP instance.</p>
  </li>
  <li>
    <p>Inside the VM, download and install the Codex CLI.</p>
  </li>
  <li>
    <p>Happy coding!</p>
  </li>
</ol>


Follow me on Twitter <a href="https://x.com/josh_bickett">@josh_bickett</a>. If you wish this was easier, please DM me on Twitter and tell me. This will motivate me to make it better :)
