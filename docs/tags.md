# Tags

{% if tags %}
  {% for tag in tags %}
    <!-- Hiển thị tag -->
  {% endfor %}
{% else %}
  <!-- Xử lý trường hợp không có tags -->
{% endif %}