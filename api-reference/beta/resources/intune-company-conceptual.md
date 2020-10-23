---
title: Microsoft Intune 中的公司条款和条件-Microsoft Graph API
description: 列出用于定义租户组织的条款和条件 (REST) 的适用于 Intune 终结点的 Microsoft Graph API。
localization_priority: Normal
author: dougeby
ms.prod: intune
ms.openlocfilehash: 439fd1b4a59a196057210aafd56d9a938573cc45
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723967"
---
# <a name="company-terms-and-conditions-in-microsoft-intune"></a>Microsoft Intune 中的公司条款和条件

命名空间：microsoft.graph

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

你可以将 Intune 条款和条件部署到用户组，以说明注册、访问工作资源和公司门户应用对设备和用户有何影响。 用户必须接受条款和条件，才能使用公司门户注册和访问其工作。

你可以创建和部署多个包含不同条款和条件的策略。 也可以生成相同条款和条件的不同语言版本，并将其部署到相应组。

以下 Graph 资源可用于管理 Intune 中的公司条款和条件：

- [条款和条件](intune-companyterms-termsandconditions.md)
- [条款和条件接受状态](intune-companyterms-termsandconditionsacceptancestatus.md)
- [条款和条件分配](intune-companyterms-termsandconditionsassignment.md)
- [条款和条件组分配](intune-companyterms-termsandconditionsgroupassignment.md)