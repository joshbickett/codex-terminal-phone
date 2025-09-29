# Running Codex in a Terminal From Your Phone

I love Codex CLI. I recently wondered if I could run it from my phone. There is ChatGPT iOS Codex, but that comes with limitations where if I run Codex CLI in a terminal from my phone I could do **anything**. For example, I built the initial version of this repo from my phone in the terminal with Codex. I asked codex to make the markdown file and add the steps. Then I described the steps as you'll see below. Furthermore I **recorded** this codex prompt so that you can see below. I SFTPed it from my phone to codex terminal and then asked codex to 6 times the speed of the record. Lastly it pushed it up so you could see the demo below!

## Workflow Demo (6× speed)

<p align="center">
  <img src="ScreenRecording_09-28-2025_21-14-54_1_speed6.gif" alt="Codex Terminal Phone workflow demo (6× speed)" width="280">
</p>


## Setup Steps

<ol>
  <li>
    <p>Launch a free GCP <code>e2-micro</code> Compute Engine VM and grab its external IP.</p>
    <p align="center">
      <img src="gcp.png" alt="Creating an e2-micro VM in GCP" width="600">
    </p>
  </li>
  <li>
    <p>Install Termius on iOS, add the VM as a host (username, SSH key, IP), and save.</p>
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
