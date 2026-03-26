# Pilot student

<i class="fa-solid fa-plane-circle-check"></i> Based at Aix-les-Milles (LFMA), France.

## METAR
<pre id="wx-metar" class="wx-raw" style="white-space: pre-wrap; word-break: break-word;">Loading…</pre>

## TAF
<pre id="wx-taf" class="wx-raw" style="white-space: pre-wrap; word-break: break-word;">Loading…</pre>

<script>
(function () {
  var API = 'https://api.allorigins.win/raw?url=https://aviationweather.gov/api/data/metar?ids=LFML&hours=0&sep=true&taf=true&format=json';
  var metarEl = document.getElementById('wx-metar');
  var tafEl = document.getElementById('wx-taf');
  if (!metarEl || !tafEl) return;
  fetch(API)
    .then(function (r) { return r.json(); })
    .then(function (data) {
      var row = Array.isArray(data) && data[0] ? data[0] : null;
      if (!row) {
        metarEl.textContent = 'No METAR data available.';
        tafEl.textContent = 'No TAF data available.';
        return;
      }
      metarEl.textContent = row.rawOb || '—';
      tafEl.textContent = row.rawTaf || '—';
    })
    .catch(function () {
      metarEl.textContent = 'Could not load METAR (network or browser restriction).';
      tafEl.textContent = 'Could not load TAF (network or browser restriction).';
    });
})();
</script>

---

# Former DevOps Engineer

7 years in tech industry, mainly deploying cloud infrastructures.

---

## <i class="fa-solid fa-wrench"></i> Projects

### Home cluster

<img src="https://img.shields.io/github/commit-activity/t/Pyrrha/home-cluster?style=flat-square" alt="GitHub commit activity" style="vertical-align: middle;">

Applications deployed on my Kubernetes home cluster, using ArgoCD and formerly SSO.

### Calcom helm chart

<img src="https://img.shields.io/github/stars/Pyrrha/calcom-helm?style=flat-square" alt="GitHub stars" style="vertical-align: middle;"> <img src="https://img.shields.io/github/commit-activity/t/Pyrrha/calcom-helm?style=flat-square" alt="GitHub commit activity" style="vertical-align: middle;">

Helm chart for Cal.com application, using a PostgreSQL database.

---

## <i class="fa-solid fa-certificate"></i> Certifications
<a href="https://www.credly.com/badges/f594457a-f0c6-4356-b2a4-9ff5c3a45a62/public_url" target="_blank"><img src="https://images.credly.com/size/220x220/images/cd038261-9d1c-4792-bc62-3a3b5bda175c/blob" alt="Terraform Associate" width="100" height="100"></a>
<a href="https://www.credly.com/badges/441e64d9-9f85-483d-b23a-58e0262d54d7/public_url" target="_blank"><img src="https://images.credly.com/size/220x220/images/8b8ed108-e77d-4396-ac59-2504583b9d54/cka_from_cncfsite__281_29.png" alt="Badge" width="100" height="100"></a>
<a href="https://www.credly.com/badges/f81d47b4-a841-4e41-bf55-d227dbaed3a4/public_url" target="_blank"><img src="https://images.credly.com/size/220x220/images/9945dfcb-1cca-4529-85e6-db1be3782210/kubernetes-security-specialist-logo2.png" alt="Badge" width="100" height="100"></a>
<a href="https://www.credly.com/badges/599669cb-a7b6-4e0b-aebc-384c1efbb090/public_url" target="_blank"><img src="https://images.credly.com/size/220x220/images/00634f82-b07f-4bbd-a6bb-53de397fc3a6/image.png" alt="AWS Cloud Practitioner" width="100" height="100"></a>

---

## <i class="fa-solid fa-house"></i> Homelab

Redaction in progress...