# 🛠️ Jenkins Troubleshooting

## Jenkins not starting

Check:

```bash
systemctl status jenkins
journalctl -u jenkins

Port already in use
Fix: sudo lsof -i :8080

Permission denied (Docker)
Fix: sudo usermod -aG docker jenkins
