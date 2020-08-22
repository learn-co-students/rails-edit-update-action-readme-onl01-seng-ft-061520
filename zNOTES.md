CURRENT edit form from file app/views/articles/edit.html.erb:

<%= form_for @article do |f| %>
  <%= f.label 'Article Title' %><br>
  <%= f.text_field :title %><br>
 
  <%= f.label 'Article Description' %><br>
  <%= f.text_area :description %><br>
 
  <%= f.submit "Submit Article" %>
<% end %>


ORIGINAL edit form from file app/views/articles/edit.html.erb:

<%= form_tag articles_path do %>
    <label>Article title:</label><br>
    <%= text_field_tag :title %><br>
   
    <label>Article Description</label><br>
    <%= text_area_tag :description %><br>
   
    <%= submit_tag "Submit Article" %>
<% end %>