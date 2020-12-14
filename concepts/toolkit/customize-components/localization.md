---
title: 本地化 Microsoft Graph Toolkit组件
description: 使用 LocalizationHelper 本地化 Microsoft Graph Toolkit组件。
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 3ac9f3fe5dedeb4e1793a589778242486f3b0070
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49660091"
---
# <a name="localizing-the-microsoft-graph-toolkit-components"></a>本地化 Microsoft Graph Toolkit组件

本地化是应用程序开发的重要方面，可在全球支持具有各种语言要求的用户。

你可以本地化 Microsoft Graph Toolkit组件，以确保 UI 反映目标语言。

## <a name="use-localizationhelper-to-add-localized-strings"></a>使用 LocalizationHelper 添加本地化字符串

工具包中所有字符串未本地化，但可以通过用于本地化应用的同一过程提供你自己的本地化字符串和管理不同语言。 为了便于本地化，工具包公开 `LocalizationHelper` 了静态类。

以下示例演示如何本地化多个组件。

```ts
import { LocalizationHelper } from "@microsoft/mgt";

LocalizationHelper.strings = {
  noResultsFound: "لم نجد أي قنوات",
  _components: {
    "login": {
      signInLinkSubtitle: "login",
      signOutLinkSubtitle: "خروج",
    },
    "people-picker": {
      inputPlaceholderText: "ابدأ في كتابة الاسم",
      noResultsFound: "لم نجد أي قنوات", //collision with global defined noResultsFound will overwrite with local result
      loadingMessage: "...جار التحميل",
    },
    "teams-channel-picker": {
      inputPlaceholderText: "حدد قناة",
      noResultsFound: "local NoResultsFound Example",
      // loadingMessage: is default string "Loading..." for this example since not defined globally or locally
    },
    "tasks": {
      removeTaskSubtitle: "delete",
      cancelNewTaskSubtitle: "canceltest",
      newTaskPlaceholder: "newTaskTest",
      addTaskButtonSubtitle: "addme",
    },
    "person-card": {
      sendEmailLinkSubtitle: "ارسل بريد الكتروني",
      startChatLinkSubtitle: "ابدأ الدردشة",
      showMoreSectionButton: "أظهر المزيد", // global declaration
    },
    "person-card-contact": {
      contactSectionTitle: "اتصل",
    },
    "person-card-organization": {
      reportsToSectionTitle: "تقارير ل",
      directReportsSectionTitle: "تقارير مباشرة",
      organizationSectionTitle: "منظمة",
      youWorkWithSubSectionTitle: "انت تعمل مع",
      userWorksWithSubSectionTitle: "يعمل مع",
    },
  },
};
```

分配属性后，所有组件将自动选取新字符串并重新呈现，从而允许您动态更改 `strings` 字符串。 

可以在全局级别或每个组件设置字符串 (`_components:` 属性设置) 。

## <a name="strings"></a>字符串

### <a name="login"></a>登录

```ts
{
  signInLinkSubtitle: 'Sign In',
  signOutLinkSubtitle: 'Sign Out'
}
```

### <a name="people-picker"></a>人员选取器

```ts
{
  inputPlaceholderText: 'Start typing a name',
  noResultsFound: `We didn't find any matches.`,
  loadingMessage: 'Loading...'
}
```

### <a name="teams-channel-picker"></a>Teams-Channel-Picker

```ts
{
  inputPlaceholderText: 'Select a channel',
  noResultsFound: `We didn't find any matches.`,
  loadingMessage: 'Loading...'
}
```

### <a name="tasks"></a>任务

```ts
{
  removeTaskSubtitle: 'Delete Task',
  cancelNewTaskSubtitle: 'cancel',
  newTaskPlaceholder: 'Task...',
  addTaskButtonSubtitle: 'Add'
}
```

### <a name="tasks-base"></a>Tasks-Base

```ts
{
  removeTaskSubtitle: 'Delete Task',
  cancelNewTaskSubtitle: 'cancel',
  newTaskPlaceholder: 'Task...',
  addTaskButtonSubtitle: 'Add'
}
```

### <a name="todo"></a>Todo

```ts
{
  removeTaskSubtitle: 'Delete Task',
  cancelNewTaskSubtitle: 'cancel',
  newTaskPlaceholder: 'Task...',
  addTaskButtonSubtitle: 'Add'
}
```

### <a name="person-card"></a>人员卡片

```ts
{
  sendEmailLinkSubtitle: 'Send email',
  startChatLinkSubtitle: 'Start chat',
  showMoreSectionButton: 'Show more'
}
```

### <a name="person-card-contact"></a>Person-Card-Contact

```ts
{
  contactSectionTitle: "Contact";
}
```

### <a name="person-card-organization"></a>Person-Card-Organization

```ts
{
  reportsToSectionTitle: 'Reports to',
  directReportsSectionTitle: 'Direct reports',
  organizationSectionTitle: 'Organization',
  youWorkWithSubSectionTitle: 'You work with',
  userWorksWithSubSectionTitle: 'works with'
}
```

### <a name="person-card-messages"></a>Person-Card-Messages

```ts
{
  emailsSectionTitle: "Emails";
}
```

### <a name="person-card-files"></a>Person-Card-Files

```ts
{
  filesSectionTitle: 'Files',
  sharedTextSubtitle: 'Shared'
}
```

### <a name="person-card-profile"></a>Person-Card-Profile

```ts
{
  SkillsAndExperienceSectionTitle: 'Skills & Experience',
  AboutCompactSectionTitle: 'About',
  SkillsSubSectionTitle: 'Skills',
  LanguagesSubSectionTitle: 'Languages',
  WorkExperienceSubSectionTitle: 'Work Experience',
  EducationSubSectionTitle: 'Education',
  professionalInterestsSubSectionTitle: 'Professional Interests',
  personalInterestsSubSectionTitle: 'Personal Interests',
  birthdaySubSectionTitle: 'Birthday',
  currentYearSubtitle: 'Current'
}
```
