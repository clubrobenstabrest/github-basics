## Étape {{ step_number }} : Résultats

| Statut | Description |
| :---: | :-- |
{% for r in results_table %}
{% if r.passed %}| ✅ Réussi | {{ r.description }} |
{% else %}| ❌ À corriger | {{ r.description }} |
{% endif %}
{% endfor %}
