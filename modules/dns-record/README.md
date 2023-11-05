# Terraform Module <img src="../resources/assets/vendor/terraform/Terraform_VerticalLogo_ColorWhite_RGB.png" width="200" align="right" />

## Clouflare DNS Record

This module manages Cloudflare DNS records by determining the zone the specified domain belongs to and passing that into Cloudflare's Terraform provider resource `cloudflare_record`, when editing the zone in order to change the records.

---

## 🚧 Usage

```hcl
module "cf_dns" {
  source = "./modules/cloudflare-dns-record"

  domain           = "delta4x4.net"
  dns_record_type  = "A" 
  dns_record_name  = "subdomain"
  dns_record_value = "xxx.xxx.xxx.xxx"
}
```

---

### 📜 License

**[Proprietary](./LICENSE)**

### ✉ Contact

- **Admin**: Maximilian Gindorfer
- **E-Mail**: [maximilian.gindorfer@delta4x4.com](mailto:maximilian.gindorfer@delta4x4.com)
- **Mobile**: +49 8134 93020

### © Copyright

_Assets provided by:_ **[Design Barn Inc.](https://iconscout.com)**
