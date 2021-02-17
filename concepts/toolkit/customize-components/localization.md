---
title: 本地化 Microsoft Graph Toolkit组件
description: 使用 LocalizationHelper 本地化 Microsoft Graph Toolkit组件。
localization_priority: Normal
author: vogtn
ms.openlocfilehash: a2bd44330e3b5e9476b86c9e9cd69aadcab43467
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272522"
---
# <a name="localizing-the-microsoft-graph-toolkit-components"></a><span data-ttu-id="a4df8-103">本地化 Microsoft Graph Toolkit组件</span><span class="sxs-lookup"><span data-stu-id="a4df8-103">Localizing the Microsoft Graph Toolkit components</span></span>

<span data-ttu-id="a4df8-104">本地化是应用程序开发的重要方面，可支持具有全球各种语言要求的用户。</span><span class="sxs-lookup"><span data-stu-id="a4df8-104">Localization is an important aspect of application development to support users with various language requirements globally.</span></span>

<span data-ttu-id="a4df8-105">你可以本地化 Microsoft Graph Toolkit组件，以确保 UI 反映目标语言。</span><span class="sxs-lookup"><span data-stu-id="a4df8-105">You can localize the Microsoft Graph Toolkit components to ensure that the UI reflects the target language.</span></span>

## <a name="use-localizationhelper-to-add-localized-strings"></a><span data-ttu-id="a4df8-106">使用 LocalizationHelper 添加本地化字符串</span><span class="sxs-lookup"><span data-stu-id="a4df8-106">Use LocalizationHelper to add localized strings</span></span>

<span data-ttu-id="a4df8-107">工具包中没有本地化的字符串，但你可以提供自己的本地化字符串，并通过用于本地化应用的同一过程管理不同的语言。</span><span class="sxs-lookup"><span data-stu-id="a4df8-107">None of the strings in the toolkit are localized, but you can provide your own localized strings and manage different languages through the same process you use for localizing your app.</span></span> <span data-ttu-id="a4df8-108">为便于本地化，工具包公开 `LocalizationHelper` 静态类。</span><span class="sxs-lookup"><span data-stu-id="a4df8-108">To facilitate localization, the toolkit exposes the `LocalizationHelper` static class.</span></span>

<span data-ttu-id="a4df8-109">以下示例演示如何本地化多个组件。</span><span class="sxs-lookup"><span data-stu-id="a4df8-109">The following example shows how to localize several components.</span></span>

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

<span data-ttu-id="a4df8-110">分配属性后，所有组件将自动选取新字符串并重新呈现，从而允许您动态 `strings` `LocalizationHelper` 更改字符串。</span><span class="sxs-lookup"><span data-stu-id="a4df8-110">When the `strings` property of `LocalizationHelper` is assigned, all components will automatically pick up the new strings and re-render, allowing you to change strings dynamically.</span></span> 

<span data-ttu-id="a4df8-111">可以在全局级别或每个组件设置字符串 (`_components:` 属性) 。</span><span class="sxs-lookup"><span data-stu-id="a4df8-111">The strings can be set at a global level or per component (with the `_components:` property).</span></span>

## <a name="strings"></a><span data-ttu-id="a4df8-112">字符串</span><span class="sxs-lookup"><span data-stu-id="a4df8-112">Strings</span></span>

### <a name="login"></a><span data-ttu-id="a4df8-113">登录</span><span class="sxs-lookup"><span data-stu-id="a4df8-113">Login</span></span>

```ts
"login": {
  signInLinkSubtitle: "Sign In",
  signOutLinkSubtitle: "Sign Out"
}
```

### <a name="people-picker"></a><span data-ttu-id="a4df8-114">人员选取器</span><span class="sxs-lookup"><span data-stu-id="a4df8-114">People-Picker</span></span>

```ts
"people-picker": {
  inputPlaceholderText: "Start typing a name",
  noResultsFound: `We didn't find any matches.`,
  loadingMessage: "Loading..."
}
```

### <a name="teams-channel-picker"></a><span data-ttu-id="a4df8-115">Teams-Channel-Picker</span><span class="sxs-lookup"><span data-stu-id="a4df8-115">Teams-Channel-Picker</span></span>

```ts
"teams-channel-picker": {
  inputPlaceholderText: "Select a channel",
  noResultsFound: `We didn't find any matches.`,
  loadingMessage: "Loading..."
}
```

### <a name="tasks"></a><span data-ttu-id="a4df8-116">任务</span><span class="sxs-lookup"><span data-stu-id="a4df8-116">Tasks</span></span>

```ts
"tasks": {
  removeTaskSubtitle: "Delete Task",
  cancelNewTaskSubtitle: "cancel",
  newTaskPlaceholder: "Task...",
  addTaskButtonSubtitle: "Add"
}
```

### <a name="tasks-base"></a><span data-ttu-id="a4df8-117">Tasks-Base</span><span class="sxs-lookup"><span data-stu-id="a4df8-117">Tasks-Base</span></span>

```ts
"tasks-base": {
  removeTaskSubtitle: "Delete Task",
  cancelNewTaskSubtitle: "cancel",
  newTaskPlaceholder: "Task...",
  addTaskButtonSubtitle: "Add"
}
```

### <a name="todo"></a><span data-ttu-id="a4df8-118">Todo</span><span class="sxs-lookup"><span data-stu-id="a4df8-118">Todo</span></span>

```ts
"todo": {
  removeTaskSubtitle: "Delete Task",
  cancelNewTaskSubtitle: "cancel",
  newTaskPlaceholder: "Task...",
  addTaskButtonSubtitle: "Add"
}
```

### <a name="person-card"></a><span data-ttu-id="a4df8-119">人员卡片</span><span class="sxs-lookup"><span data-stu-id="a4df8-119">Person-Card</span></span>

```ts
"person-card": {
  sendEmailLinkSubtitle: "Send email",
  startChatLinkSubtitle: "Start chat",
  showMoreSectionButton: "Show more"
}
```

### <a name="person-card-contact"></a><span data-ttu-id="a4df8-120">Person-Card-Contact</span><span class="sxs-lookup"><span data-stu-id="a4df8-120">Person-Card-Contact</span></span>

```ts
"person-card-contact": {
  contactSectionTitle: "Contact"
}
```

### <a name="person-card-organization"></a><span data-ttu-id="a4df8-121">Person-Card-Organization</span><span class="sxs-lookup"><span data-stu-id="a4df8-121">Person-Card-Organization</span></span>

```ts
"person-card-organization": {
  reportsToSectionTitle: "Reports to",
  directReportsSectionTitle: "Direct reports",
  organizationSectionTitle: "Organization",
  youWorkWithSubSectionTitle: "You work with",
  userWorksWithSubSectionTitle: "works with"
}
```

### <a name="person-card-messages"></a><span data-ttu-id="a4df8-122">Person-Card-Messages</span><span class="sxs-lookup"><span data-stu-id="a4df8-122">Person-Card-Messages</span></span>

```ts
"person-card-messages": {
  emailsSectionTitle: "Emails"
}
```

### <a name="person-card-files"></a><span data-ttu-id="a4df8-123">Person-Card-Files</span><span class="sxs-lookup"><span data-stu-id="a4df8-123">Person-Card-Files</span></span>

```ts
"person-card-files": {
  filesSectionTitle: "Files",
  sharedTextSubtitle: "Shared"
}
```

### <a name="person-card-profile"></a><span data-ttu-id="a4df8-124">Person-Card-Profile</span><span class="sxs-lookup"><span data-stu-id="a4df8-124">Person-Card-Profile</span></span>

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
