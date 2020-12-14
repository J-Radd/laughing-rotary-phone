stripe charges retrieve ch_1Hy5V2JtofXoPBKRjzK1ZdMd \
    --stripe-account acct_1HmuxwJtofXoPBKR
'Authorization: sk_live_...4kUR'
 "id": "acct_1HmuxwJtofXoPBKR",
  "object": "account",
  "business_profile": {
    "mcc": "1520",
    "name": null,
    "product_description": "Phoenix Restorations is one of the most established local restoration companies.  Since 1981, we have been restoring strata, residential, commercial and industrial properties with exceptional service and workmanship.",
    "support_address": null,
    "support_email": null,
    "support_phone": "+16048545537",
    "support_url": null,
    "url": "https://www.phoenixrestorations.com/"
  },
  "business_type": "individual",
  "capabilities": {
    "card_payments": "active",
    "transfers": "active"
  },
  "charges_enabled": false,
  "country": "CA",
  "default_currency": "cad",
  "details_submitted": true,
  "email": "jsayers8080@gmail.com",
  "metadata": {},
  "payouts_enabled": true,
  "requirements": {
    "current_deadline": null,
    "currently_due": [],
    "disabled_reason": "rejected.fraud",
    "errors": [],
    "eventually_due": [
      "individual.verification.document"
    ],
    "past_due": [],
    "pending_verification": []
  },
  "settings": {
    "bacs_debit_payments": {},
    "branding": {
      "icon": null,
      "logo": null,
      "primary_color": null,
      "secondary_color": null
    },
    "card_payments": {
      "decline_on": {
        "avs_failure": false,
        "cvc_failure": true
      },
      "statement_descriptor_prefix": "K-192248 "
    },
    "dashboard": {
      "display_name": "Phoenixrestorations",
      "timezone": "Etc/UTC"
    },
    "payments": {
      "statement_descriptor": "(PHEOMAIN)",
      "statement_descriptor_kana": null,
      "statement_descriptor_kanji": null
    },
    "payouts": {
      "debit_negative_balances": true,
      "schedule": {
        "delay_days": 7,
        "interval": "daily"
      },
      "statement_descriptor": null
    },
    "sepa_debit_payments": {}
  },
  "type": "standard"
}
 'Authorization: sk_live_...4kUR'
curl https://api.stripe.com/v1/payouts \
  -pk_live_51HmuxwJtofXoPBKRkazCq3CdfvoklhROZ54cvnccTqSYLD7CPcRM0caLbIrAd3G1yopDpwZTZF0LPB3v9bMRVbKj00MSXeThif
  -d amount=5000 \
  -d currency=usd
  
