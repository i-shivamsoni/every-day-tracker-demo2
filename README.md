# Habit Tracker

A simple, customizable GitHub Pages-based habit tracking system. Track your daily habits with colorful visualizations and easy journal entries.

**[View Demo](https://i-shivamsoni.github.io/every-day-tracker-demo2/)**

## Getting Started

### Setup Your Repository

1. Click the **Use this template** button in the top right corner of this repository
2. Select **Create a new repository**
3. Give your repository a name (e.g., `my-habit-tracker`)
4. Choose public or private visibility (GitHub Pages works with both)
5. Click **Create repository**

### Enable GitHub Pages

1. Go to your new repository's **Settings** tab
2. Scroll down to the **GitHub Pages** section
3. Under **Source**, select the branch (usually `main`) and folder (usually `/root`)
4. Click **Save**
5. Wait a few minutes for your site to be published
6. Access your habit tracker at `https://yourusername.github.io/your-repo-name/`

## Customizing Your Habits

### Configure Your Habits

Edit the `_config.yml` file to customize your habits and their colors:

```yaml
habits:
  gym: "#4A9DFF"         # Bright blue - energetic and active
  meals: "#50C878"       # Emerald green - fresh and healthy
  work: "#FF6B6B"        # Coral pink - productive and focused
  reading: "#FFD93D"     # Warm yellow - knowledge and learning
  meditation: "#9D8CFF"  # Soft purple - calm and mindful
  sleep: "#614BC3"       # Deep purple - restful and peaceful
```

Feel free to change the habit names and colors to match your preferences. Some additional color suggestions are included as comments.

## Adding Habit Entries

### Create Folder Structure

For each habit defined in your `_config.yml`, create a matching folder in the `_posts` directory:

```
_posts/
  ├── gym/
  ├── meals/
  ├── work/
  ├── reading/
  ├── meditation/
  └── sleep/
```

### Create Daily Entries

1. Inside each habit folder, create files using this naming format:
   ```
   YYYY-MM-DD-habit-name.md
   ```
   
   For example:
   ```
   2025-02-25-gym.md
   ```

2. Add the required metadata at the top of each file:
   ```markdown
   ---
   date: 2025-02-25
   title: "Morning Workout"
   category: gym
   description: "45-minute strength training"
   ---
   
   Had a great morning workout focusing on upper body. Completed 3 sets of bench press, shoulder press, and pull-ups. Feeling energized for the day!
   ```

   Make sure the `category` matches exactly with the habit name in your `_config.yml`.

## Tips for Success

1. **Consistent naming**: Ensure folder names and category values match exactly with habit names in `_config.yml`
2. **Regular updates**: Create new entries daily to maintain your habit tracking
3. **Meaningful descriptions**: Use the description field for quick summaries
4. **Detailed content**: Add as much detail as you want after the metadata section
5. **Git workflow**: You can update your tracker:
   - Directly on GitHub by creating/editing files in your repository
   - Locally using Git commands:
     ```
     git clone https://github.com/yourusername/your-repo-name.git
     # Make your changes
     git add .
     git commit -m "Add today's entries"
     git push
     ```

## Troubleshooting

- **Changes not appearing?** GitHub Pages may take a few minutes to update
- **Colors not showing?** Check that habit names in `_config.yml` match folder and category names exactly
- **Page not found?** Ensure GitHub Pages is properly enabled in repository settings

## Customizing Further

- Edit the CSS in `assets/css/style.scss` to change the appearance
- Modify template files in `_layouts/` to change the structure
- Add additional features like tags, search, or statistics by extending the Jekyll configuration

---

Happy habit tracking!
