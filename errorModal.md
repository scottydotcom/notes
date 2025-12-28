error handling modal example

```html
<section class="error-message">
  <h1>Unable to connect your account</h1>
  <p>
    Your changes were saved, but we could not connect your account due to a technical issue on our end. Please try
    connecting again. If the issue keeps happening,
    <a href="mailto:customercare@example.com" style="text-decoration: underline;">contact Customer Care</a>.
  </p>
  <div class="error-actions">
    <button type="button" class="cancel-button">Cancel</button>
    <button type="button" class="try-again-button">Try Again</button>
  </div>
</section>
```

```css
/* Custom CSS to mimic Bootstrap's rounded card styling */

.error-message {
  border: 1px solid #dee2e6; /* Mimics Bootstrap's card border */
  border-radius: 0.375rem; /* Mimics Bootstrap's .rounded */
  padding: 1rem; /* Mimics Bootstrap's .p-3 */
  background-color: #fff; /* White background for card-like appearance */
  box-shadow: 0 0.125rem 0.25rem rgba(0, 0, 0, 0.075); /* Mimics Bootstrap's card shadow */
  margin: 1rem; /* Optional: Add some margin for spacing */
}

.error-actions {
  display: flex;
  justify-content: center;
  gap: 0.5rem; /* Mimics Bootstrap's .gap-2 */
}

.cancel-button, .try-again-button {
  border-radius: 0.375rem; /* Mimics Bootstrap's .rounded on buttons */
  padding: 0.375rem 0.75rem; /* Mimics Bootstrap button padding */
  font-size: 1rem;
  line-height: 1.5;
  text-align: center;
  text-decoration: none;
  vertical-align: middle;
  cursor: pointer;
  transition: color 0.15s ease-in-out, background-color 0.15s ease-in-out, border-color 0.15s ease-in-out, box-shadow 0.15s ease-in-out;
  border: 1px solid; /* Base border for both */
}

.cancel-button {
  color: #dc3545; /* Red text */
  background-color: #fff; /* White background */
  border-color: #dc3545; /* Red outline */
}

.cancel-button:hover {
  color: #fff;
  background-color: #dc3545; /* Red background on hover */
  border-color: #dc3545;
}

.try-again-button {
  color: #fff; /* White text */
  background-color: #dc3545; /* Red background */
  border-color: #dc3545; /* Red border (though it blends with bg) */
}

.try-again-button:hover {
  color: #fff;
  background-color: #c82333; /* Darker red on hover */
  border-color: #bd2130;
}
```