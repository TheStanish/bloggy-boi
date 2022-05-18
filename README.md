# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...
# alpha-blog

discarded code:

<%= link_to 'Articles Listing', articles_path %> |
<%= link_to 'About Page', about_path %>

<table>
  <thead>
    <tr>
      <th>Title</th>
      <th>Description</th>
      <th colspan="3">Actions</th>
    </tr>
  </thead>

  <tbody>
    <% @articles.each do |article| %>
      <tr>
        <td> <%= article.title %> </td>
        <td> <%= article.description %> </td>
        <td><%= link_to 'Show', article_path(article) %></td>
        <td><%= link_to 'Edit', edit_article_path(article) %></td>
        <td><%= link_to 'Delete', article_path(article), method: :delete, data: { confirm: "Are you sure?"} %></td>
      </tr>
    <% end %>
  </tbody>
</table>

<p>
<%= link_to 'Create New Article', new_article_path %> |
<%= link_to 'Home Page', root_path %> |
<%= link_to 'About Page', about_path %>
</p>
