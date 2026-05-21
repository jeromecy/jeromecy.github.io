---
layout: page
permalink: /contact/
description: "Contact Dr. Zhanglong Cao for research collaborations, speaking opportunities, and statistical consultation in agricultural research and data analytics."
---

<div class="hero">
  <h1>Get in Touch</h1>
  <p>I'm always interested in new research collaborations, speaking opportunities, and discussions about statistical methodology in agriculture.</p>
</div>

<div class="contact-container">
  <!-- Left Column: Contact Form -->
  <div class="contact-form-section">
    <div class="form-card">
      <h2>📧 Send a Message</h2>
      <form action="https://formspree.io/f/xayzqjqj" method="POST" class="contact-form">
        <div class="form-group">
          <label for="name">Name *</label>
          <input type="text" id="name" name="name" required class="form-control">
        </div>
        
        <div class="form-group">
          <label for="email">Email *</label>
          <input type="email" id="email" name="email" required class="form-control">
        </div>
        
        <div class="form-group">
          <label for="subject">Subject</label>
          <select id="subject" name="subject" class="form-control">
            <option value="">Select a topic...</option>
            <option value="research-collaboration">Research Collaboration</option>
            <option value="speaking-opportunity">Speaking Opportunity</option>
            <option value="student-supervision">Student Supervision</option>
            <option value="consultation">Statistical Consultation</option>
            <option value="other">Other</option>
          </select>
        </div>
        
        <div class="form-group">
          <label for="message">Message *</label>
          <textarea id="message" name="message" rows="6" required class="form-control" placeholder="Please describe your inquiry..."></textarea>
        </div>
        
        <button type="submit" class="btn btn-primary">Send Message</button>
      </form>
    </div>
  </div>

  <!-- Right Column: Contact Information -->
  <div class="contact-info-section">
    <!-- Direct Contact -->
    <div class="info-card">
      <h3>📍 Direct Contact</h3>
      <div class="contact-item">
        <div class="contact-icon">📧</div>
        <div class="contact-details">
          <h4>Email</h4>
          <p><a href="mailto:{{ site.author.email }}">{{ site.author.email }}</a></p>
          <p><a href="mailto:zhanglong.cao@curtin.edu.au">zhanglong.cao@curtin.edu.au</a></p>
        </div>
      </div>
      
      <div class="contact-item">
        <div class="contact-icon">🏢</div>
        <div class="contact-details">
          <h4>Office</h4>
          <p><strong>Curtin University</strong></p>
          <p>Perth, Western Australia</p>
          <p>Australia</p>
        </div>
      </div>
    </div>

    <!-- Professional Profiles -->
    <div class="info-card">
      <h3>🔗 Professional Profiles</h3>
      <div class="profile-links">
        <a href="https://github.com/{{ site.author.github }}" class="profile-link">
          <span class="profile-icon">🐙</span>
          <span>GitHub</span>
        </a>
        <a href="https://linkedin.com/in/{{ site.author.linkedin }}" class="profile-link">
          <span class="profile-icon">💼</span>
          <span>LinkedIn</span>
        </a>
        <a href="https://www.researchgate.net/profile/Zhanglong-Cao" class="profile-link">
          <span class="profile-icon">🔬</span>
          <span>ResearchGate</span>
        </a>
      </div>
    </div>

    <!-- Collaboration Areas -->
    <div class="info-card">
      <h3>🤝 Collaboration Areas</h3>
      <div class="collaboration-areas">
        <div class="area-item">
          <h4>📊 Research Projects</h4>
          <ul>
            <li>Agricultural Statistics</li>
            <li>Bayesian Methods</li>
            <li>Machine Learning</li>
            <li>Software Development</li>
          </ul>
        </div>
        
        <div class="area-item">
          <h4>🎤 Speaking & Teaching</h4>
          <ul>
            <li>Conference Presentations</li>
            <li>Workshops</li>
            <li>Guest Lectures</li>
            <li>Industry Training</li>
          </ul>
        </div>
      </div>
    </div>

    <!-- Services -->
    <div class="info-card">
      <h3>💼 Professional Services</h3>
      <div class="services-list">
        <div class="service-item">
          <span class="service-icon">📈</span>
          <span>Statistical Consulting</span>
        </div>
        <div class="service-item">
          <span class="service-icon">🔬</span>
          <span>Experimental Design</span>
        </div>
        <div class="service-item">
          <span class="service-icon">💻</span>
          <span>Software Development</span>
        </div>
        <div class="service-item">
          <span class="service-icon">📝</span>
          <span>Report Writing</span>
        </div>
      </div>
    </div>
  </div>
</div> 