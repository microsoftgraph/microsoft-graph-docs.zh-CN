---
title: Microsoft Intune 中的公司条款和条件 - Microsoft Graph API
description: 列出支持Graph公司条款和条件的 Microsoft Graph API (REST) 终结点。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 0a67f9704e68e75a1875cad16a3fca91e97081fe
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53108850"
---
# <a name="company-terms-and-conditions-in-microsoft-intune"></a>Microsoft Intune 中的公司条款和条件

命名空间：microsoft.graph

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户 [正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。

你可以将 Intune 条款和条件部署到用户组，以说明注册、访问工作资源和公司门户应用对设备和用户有何影响。 用户必须接受条款和条件，才能使用公司门户注册和访问其工作。

你可以创建和部署多个包含不同条款和条件的策略。 也可以生成相同条款和条件的不同语言版本，并将其部署到相应组。

以下 Graph 资源可用于管理 Intune 中的公司条款和条件：

- [设备管理](intune-companyterms-devicemanagement.md)
- [条款和条件](intune-companyterms-termsandconditions.md)
- [条款和条件接受状态](intune-companyterms-termsandconditionsacceptancestatus.md)
- [条款和条件分配](intune-companyterms-termsandconditionsassignment.md)