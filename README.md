# Running Codex in a Terminal From Your Phone

## Workflow Demo (6× speed)

<p align="center">
  <img src="ScreenRecording_09-28-2025_21-14-54_1_speed6.gif" alt="Codex Terminal Phone workflow demo (6× speed)" width="280">
</p>

<p align="center">
  <a href="ScreenRecording_09-28-2025%2021-14-54_1_speed6.mp4">Download the full video with audio</a>
</p>

## Setup Steps

<ol>
  <li>
    <p>Launch a free GCP <code>e2-micro</code> Compute Engine VM and grab its external IP.</p>
    <p align="center">
      <img src="gcp.png" alt="Creating an e2-micro VM in GCP" width="760">
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
