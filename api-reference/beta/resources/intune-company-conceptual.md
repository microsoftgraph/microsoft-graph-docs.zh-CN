---
title: Microsoft Intune 中的公司条款和条件 - Microsoft Graph API
description: 列出定义Graph条款和条件的适用于 Intune 终结点的 Microsoft (API) REST 应用程序。
localization_priority: Normal
author: dougeby
ms.prod: intune
ms.openlocfilehash: 59d72416edb38872effd4dcca2a3a898e86bcfb9bf30f131c0ee0b43f8443769
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54170445"
---
# <a name="company-terms-and-conditions-in-microsoft-intune"></a>Microsoft Intune 中的公司条款和条件

命名空间：microsoft.graph

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

你可以将 Intune 条款和条件部署到用户组，以说明注册、访问工作资源和公司门户应用对设备和用户有何影响。 用户必须接受条款和条件，才能使用公司门户注册和访问其工作。

你可以创建和部署多个包含不同条款和条件的策略。 也可以生成相同条款和条件的不同语言版本，并将其部署到相应组。

以下 Graph 资源可用于管理 Intune 中的公司条款和条件：

- [条款和条件](intune-companyterms-termsandconditions.md)
- [条款和条件接受状态](intune-companyterms-termsandconditionsacceptancestatus.md)
- [条款和条件分配](intune-companyterms-termsandconditionsassignment.md)
- [条款和条件组分配](intune-companyterms-termsandconditionsgroupassignment.md)