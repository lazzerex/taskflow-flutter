# TaskFlow Flutter

A modern task management application built with Flutter, ported from the original Laravel web application. TaskFlow provides an intuitive interface for organizing and tracking daily tasks with features like priority levels, categories, and progress monitoring.

## About

This is a Flutter port of the original TaskFlow web application that was built with Laravel. The mobile version maintains the core functionality while providing a native mobile experience with offline capabilities and responsive design.

## Features

**Task Management**
- Create, edit, and delete tasks
- Mark tasks as complete or incomplete
- Set task priorities (Low, Medium, High)
- Organize tasks by categories (Personal, Work, Shopping, Health, Other)
- Optional due dates with visual indicators

**Dashboard and Analytics**
- Real-time task statistics
- Progress tracking with completion percentages
- Filter tasks by status and priority
- Overview of total, completed, and pending tasks

**User Interface**
- Clean and modern Material Design 3 interface
- Dark and light theme support
- Responsive design for various screen sizes
- Smooth animations and intuitive navigation

**Data Management**
- Local data persistence using SharedPreferences
- Offline functionality - no internet connection required
- Automatic data saving and loading
- JSON-based data serialization

## Technology Stack

- **Framework**: Flutter 3.0+
- **Language**: Dart
- **Storage**: SharedPreferences (local storage)
- **Fonts**: Google Fonts (Inter)
- **Architecture**: MVC pattern with services layer
- **Testing**: Flutter testing framework

## Getting Started

### Prerequisites
- Flutter SDK 3.0.0 or higher
- Dart SDK
- Android Studio or VS Code with Flutter extensions
- Chrome browser (for web development)

### Installation

1. Clone the repository
   ```bash
   git clone https://github.com/lazzerex/taskflow-flutter.git
   cd taskflow-flutter
   ```

2. Install dependencies
   ```bash
   flutter pub get
   ```

3. Run the application
   ```bash
   flutter run
   ```

### Available Platforms
- Android
- iOS
- Web
- Windows/macOS/Linux (desktop)

## Project Structure

```
lib/
├── main.dart                 # Application entry point
├── models/
│   └── task.dart            # Task data model with JSON serialization
├── services/
│   └── task_service.dart    # Data persistence and business logic
├── screens/
│   ├── home_screen.dart     # Main dashboard with task list
│   └── add_task_screen.dart # Task creation and editing interface
├── widgets/
│   ├── task_card.dart       # Individual task display component
│   └── stats_card.dart      # Statistics display component
└── theme/
    └── app_theme.dart       # Application theming and styles
```

## Dependencies

- `flutter`: Flutter SDK
- `google_fonts`: Typography and font management
- `shared_preferences`: Local data persistence
- `intl`: Date formatting and internationalization

## Development

### Running Tests
```bash
flutter test
```

### Building for Production
```bash
# Android
flutter build apk

# iOS
flutter build ios

# Web
flutter build web
```

### Code Style
This project follows standard Dart and Flutter conventions. Use the following commands to maintain code quality:

```bash
flutter analyze
dart format .
```

## Differences from Laravel Version

The Flutter version includes several mobile-specific enhancements:

- **Offline-first architecture**: Works without internet connection
- **Touch-optimized interface**: Designed for mobile interaction patterns
- **Local storage**: Data persisted locally using SharedPreferences
- **Cross-platform support**: Runs on mobile, web, and desktop
- **Material Design**: Native mobile UI components and patterns

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Development Guidelines
- Follow Flutter and Dart best practices
- Write tests for new features
- Update documentation for significant changes
- Ensure compatibility across supported platforms

## Roadmap

**Planned Features**
- Cloud synchronization with backend API
- Push notifications for task reminders
- Task sharing and collaboration features
- Advanced filtering and search capabilities
- Data export functionality
- Widget support for home screen
- Task templates and recurring tasks

**Technical Improvements**
- State management with Provider/Bloc
- Integration with calendar applications
- Biometric authentication
- Advanced analytics and reporting

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Original Laravel web application that inspired this mobile port
- Flutter team for the excellent framework and documentation
- Google Fonts for typography resources
- Material Design team for UI/UX guidelines

## Support

For bug reports and feature requests, please use the GitHub Issues page. For general questions about implementation or usage, feel free to open a discussion.

## Links

- Original Laravel Version: https://github.com/lazzerex/task-flow
- Flutter Documentation: https://flutter.dev/docs
- Dart Language: https://dart.dev