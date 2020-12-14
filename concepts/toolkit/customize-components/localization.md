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
# <a name="localizing-the-microsoft-graph-toolkit-components"></a><span data-ttu-id="f34e5-103">本地化 Microsoft Graph Toolkit组件</span><span class="sxs-lookup"><span data-stu-id="f34e5-103">Localizing the Microsoft Graph Toolkit components</span></span>

<span data-ttu-id="f34e5-104">本地化是应用程序开发的重要方面，可在全球支持具有各种语言要求的用户。</span><span class="sxs-lookup"><span data-stu-id="f34e5-104">Localization is a important aspect of application development to support users with various language requirements globally.</span></span>

<span data-ttu-id="f34e5-105">你可以本地化 Microsoft Graph Toolkit组件，以确保 UI 反映目标语言。</span><span class="sxs-lookup"><span data-stu-id="f34e5-105">You can localize the Microsoft Graph Toolkit components to ensure that the UI reflects the target language.</span></span>

## <a name="use-localizationhelper-to-add-localized-strings"></a><span data-ttu-id="f34e5-106">使用 LocalizationHelper 添加本地化字符串</span><span class="sxs-lookup"><span data-stu-id="f34e5-106">Use LocalizationHelper to add localized strings</span></span>

<span data-ttu-id="f34e5-107">工具包中所有字符串未本地化，但可以通过用于本地化应用的同一过程提供你自己的本地化字符串和管理不同语言。</span><span class="sxs-lookup"><span data-stu-id="f34e5-107">All strings in the toolkit are not localized, but you can provide your own localized strings and manage different languages through the same process you use for localizing your app.</span></span> <span data-ttu-id="f34e5-108">为了便于本地化，工具包公开 `LocalizationHelper` 了静态类。</span><span class="sxs-lookup"><span data-stu-id="f34e5-108">To facilitate localization, the toolkit exposes the `LocalizationHelper` static class.</span></span>

<span data-ttu-id="f34e5-109">以下示例演示如何本地化多个组件。</span><span class="sxs-lookup"><span data-stu-id="f34e5-109">The following example shows how to localize several components.</span></span>

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

<span data-ttu-id="f34e5-110">分配属性后，所有组件将自动选取新字符串并重新呈现，从而允许您动态更改 `strings` 字符串。</span><span class="sxs-lookup"><span data-stu-id="f34e5-110">When the `strings` property is assigned, all components will automatically pick up the new strings and re-render, allowing you to change strings dynamically.</span></span> 

<span data-ttu-id="f34e5-111">可以在全局级别或每个组件设置字符串 (`_components:` 属性设置) 。</span><span class="sxs-lookup"><span data-stu-id="f34e5-111">The strings can be set at a global level or per component (with the `_components:` property).</span></span>

## <a name="strings"></a><span data-ttu-id="f34e5-112">字符串</span><span class="sxs-lookup"><span data-stu-id="f34e5-112">Strings</span></span>

### <a name="login"></a><span data-ttu-id="f34e5-113">登录</span><span class="sxs-lookup"><span data-stu-id="f34e5-113">Login</span></span>

```ts
{
  signInLinkSubtitle: 'Sign In',
  signOutLinkSubtitle: 'Sign Out'
}
```

### <a name="people-picker"></a><span data-ttu-id="f34e5-114">人员选取器</span><span class="sxs-lookup"><span data-stu-id="f34e5-114">People-Picker</span></span>

```ts
{
  inputPlaceholderText: 'Start typing a name',
  noResultsFound: `We didn't find any matches.`,
  loadingMessage: 'Loading...'
}
```

### <a name="teams-channel-picker"></a><span data-ttu-id="f34e5-115">Teams-Channel-Picker</span><span class="sxs-lookup"><span data-stu-id="f34e5-115">Teams-Channel-Picker</span></span>

```ts
{
  inputPlaceholderText: 'Select a channel',
  noResultsFound: `We didn't find any matches.`,
  loadingMessage: 'Loading...'
}
```

### <a name="tasks"></a><span data-ttu-id="f34e5-116">任务</span><span class="sxs-lookup"><span data-stu-id="f34e5-116">Tasks</span></span>

```ts
{
  removeTaskSubtitle: 'Delete Task',
  cancelNewTaskSubtitle: 'cancel',
  newTaskPlaceholder: 'Task...',
  addTaskButtonSubtitle: 'Add'
}
```

### <a name="tasks-base"></a><span data-ttu-id="f34e5-117">Tasks-Base</span><span class="sxs-lookup"><span data-stu-id="f34e5-117">Tasks-Base</span></span>

```ts
{
  removeTaskSubtitle: 'Delete Task',
  cancelNewTaskSubtitle: 'cancel',
  newTaskPlaceholder: 'Task...',
  addTaskButtonSubtitle: 'Add'
}
```

### <a name="todo"></a><span data-ttu-id="f34e5-118">Todo</span><span class="sxs-lookup"><span data-stu-id="f34e5-118">Todo</span></span>

```ts
{
  removeTaskSubtitle: 'Delete Task',
  cancelNewTaskSubtitle: 'cancel',
  newTaskPlaceholder: 'Task...',
  addTaskButtonSubtitle: 'Add'
}
```

### <a name="person-card"></a><span data-ttu-id="f34e5-119">人员卡片</span><span class="sxs-lookup"><span data-stu-id="f34e5-119">Person-Card</span></span>

```ts
{
  sendEmailLinkSubtitle: 'Send email',
  startChatLinkSubtitle: 'Start chat',
  showMoreSectionButton: 'Show more'
}
```

### <a name="person-card-contact"></a><span data-ttu-id="f34e5-120">Person-Card-Contact</span><span class="sxs-lookup"><span data-stu-id="f34e5-120">Person-Card-Contact</span></span>

```ts
{
  contactSectionTitle: "Contact";
}
```

### <a name="person-card-organization"></a><span data-ttu-id="f34e5-121">Person-Card-Organization</span><span class="sxs-lookup"><span data-stu-id="f34e5-121">Person-Card-Organization</span></span>

```ts
{
  reportsToSectionTitle: 'Reports to',
  directReportsSectionTitle: 'Direct reports',
  organizationSectionTitle: 'Organization',
  youWorkWithSubSectionTitle: 'You work with',
  userWorksWithSubSectionTitle: 'works with'
}
```

### <a name="person-card-messages"></a><span data-ttu-id="f34e5-122">Person-Card-Messages</span><span class="sxs-lookup"><span data-stu-id="f34e5-122">Person-Card-Messages</span></span>

```ts
{
  emailsSectionTitle: "Emails";
}
```

### <a name="person-card-files"></a><span data-ttu-id="f34e5-123">Person-Card-Files</span><span class="sxs-lookup"><span data-stu-id="f34e5-123">Person-Card-Files</span></span>

```ts
{
  filesSectionTitle: 'Files',
  sharedTextSubtitle: 'Shared'
}
```

### <a name="person-card-profile"></a><span data-ttu-id="f34e5-124">Person-Card-Profile</span><span class="sxs-lookup"><span data-stu-id="f34e5-124">Person-Card-Profile</span></span>

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
