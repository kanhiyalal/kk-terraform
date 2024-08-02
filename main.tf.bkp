provider "google" {
  project = "projectkk-terraform"
  region  = "us-central1"
}

resource "google_compute_instance" "vm_instance" {
  name         = "my-instance"
  machine_type = "n1-standard-1"
  zone         = "us-central1-a"


  boot_disk {
    initialize_params {
      image = "debian-cloud/debian-10-buster-v20210817"
    }
  }

network_interface {
    network = "default"
    access_config {}
  }
}
