---
title: 本地化 Microsoft Graph Toolkit组件
description: 使用 LocalizationHelper 本地化 Microsoft Graph Toolkit组件。
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 934873a6695ce2e858173e0a8f965a7762805c76
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589231"
---
# <a name="localizing-the-microsoft-graph-toolkit-components"></a>本地化 Microsoft Graph Toolkit组件

本地化是应用程序开发的重要方面，可在全球支持具有各种语言要求的用户。

你可以本地化 Microsoft Graph Toolkit组件，以确保 UI 反映目标语言。

## <a name="use-localizationhelper-to-add-localized-strings"></a>使用 LocalizationHelper 添加本地化字符串

工具包中没有本地化的字符串，但你可以提供你自己的本地化字符串，并通过用于本地化应用的同一过程管理不同的语言。 为便于本地化，工具包公开静态 `LocalizationHelper` 类。

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
      noResultsFound: "لم نجد أي قنوات", // will overwrite globally defined noResultsFound in people-picker component
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
      showExpandedDetailsButton: 'Show expanded details',
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

`strings`分配 的属性后`LocalizationHelper`，所有组件将自动选取新字符串并重新呈现，从而允许您动态更改字符串。 

字符串可以在全局级别设置，也可以按组件设置 (属性 `_components:` 设置) 。

## <a name="strings"></a>字符串

### <a name="login"></a>登录

```ts
"login": {
  signInLinkSubtitle: "Sign In",
  signOutLinkSubtitle: "Sign Out"
}
```

### <a name="people-picker"></a>人员选取器

```ts
"people-picker": {
  inputPlaceholderText: "Start typing a name",
  noResultsFound: `We didn't find any matches.`,
  loadingMessage: "Loading..."
}
```

### <a name="teams-channel-picker"></a>Teams-Channel-Picker

```ts
"teams-channel-picker": {
  inputPlaceholderText: "Select a channel",
  noResultsFound: `We didn't find any matches.`,
  loadingMessage: "Loading..."
}
```

### <a name="tasks"></a>任务

```ts
"tasks": {
  removeTaskSubtitle: "Delete Task",
  cancelNewTaskSubtitle: "cancel",
  newTaskPlaceholder: "Task...",
  addTaskButtonSubtitle: "Add"
}
```

### <a name="tasks-base"></a>Tasks-Base

```ts
"tasks-base": {
  removeTaskSubtitle: "Delete Task",
  cancelNewTaskSubtitle: "cancel",
  newTaskPlaceholder: "Task...",
  addTaskButtonSubtitle: "Add"
}
```

### <a name="todo"></a>Todo

```ts
"todo": {
  removeTaskSubtitle: "Delete Task",
  cancelNewTaskSubtitle: "cancel",
  newTaskPlaceholder: "Task...",
  addTaskButtonSubtitle: "Add"
}
```

### <a name="person-card"></a>人员卡片

```ts
"person-card": {
  sendEmailLinkSubtitle: "Send email",
  startChatLinkSubtitle: "Start chat",
  showMoreSectionButton: "Show more"
}
```

### <a name="person-card-contact"></a>Person-Card-Contact

```ts
"person-card-contact": {
  contactSectionTitle: "Contact"
}
```

### <a name="person-card-organization"></a>Person-Card-Organization

```ts
"person-card-organization": {
  reportsToSectionTitle: "Reports to",
  directReportsSectionTitle: "Direct reports",
  organizationSectionTitle: "Organization",
  youWorkWithSubSectionTitle: "You work with",
  userWorksWithSubSectionTitle: "works with"
}
```

### <a name="person-card-messages"></a>Person-Card-Messages

```ts
"person-card-messages": {
  emailsSectionTitle: "Emails"
}
```

### <a name="person-card-files"></a>Person-Card-Files

```ts
"person-card-files": {
  filesSectionTitle: "Files",
  sharedTextSubtitle: "Shared"
}
```

### <a name="person-card-profile"></a>Person-Card-Profile

```ts
"person-card-profile": {
  SkillsAndExperienceSectionTitle: "Skills & Experience",
  AboutCompactSectionTitle: "About",
  SkillsSubSectionTitle: "Skills",
  LanguagesSubSectionTitle: "Languages",
  WorkExperienceSubSectionTitle: "Work Experience",
  EducationSubSectionTitle: "Education",
  professionalInterestsSubSectionTitle: "Professional Interests",
  personalInterestsSubSectionTitle: "Personal Interests",
  birthdaySubSectionTitle: "Birthday",
  currentYearSubtitle: "Current"
}
```

### <a name="file"></a>文件

```ts
'file': {
  modifiedSubtitle: 'Modified',
  sizeSubtitle: 'Size'
};
```

### <a name="file-list"></a>File-List

```ts
"file-list": {
  showMoreSubtitle: 'Show more items'
}
```
