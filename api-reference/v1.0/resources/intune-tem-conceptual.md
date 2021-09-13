---
title: Microsoft Intune 中的电信费用管理
description: 使用 Saaswedo 电信费用管理服务时，你可以在企业拥有的设备上限制数据使用和漫游，它会与 Intune 集成。 该服务让你可以设置和强制执行使用限制，并在超过配置的阈值时向用户发送警报。 用户超过阈值时，你还可以配置服务以采取其他操作，例如禁用漫游。 Saaswedo 控制台中提供包含数据使用情况和监视信息的报告。 通过 Intune 使用 Saaswedo 电信费用管理服务之前，你需要在 Saaswedo 控制台和 Intune 中配置设置。 必须打开 Saaswedo 服务和 Intune 的连接。 如果启用了 Saaswedo 端的连接，但未启用 Intune 端的连接，Intune 会忽略接收到的通信。
ms.localizationpriority: medium
author: dougeby
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: bca0c45cd2ed6bd6d556c60335e95a7d18122144
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59021573"
---
# <a name="telecom-expense-management-in-microsoft-intune"></a>Microsoft Intune 中的电信费用管理

命名空间：microsoft.graph

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户 [正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。

使用 Saaswedo 电信费用管理服务时，你可以在企业拥有的设备上限制数据使用和漫游，它会与 Intune 集成。 该服务让你可以设置和强制执行使用限制，并在超过配置的阈值时向用户发送警报。 用户超过阈值时，你还可以配置服务以采取其他操作，例如禁用漫游。 Saaswedo 控制台中提供包含数据使用情况和监视信息的报告。 通过 Intune 使用 Saaswedo 电信费用管理服务之前，你需要在 Saaswedo 控制台和 Intune 中配置设置。 必须打开 Saaswedo 服务和 Intune 的连接。 如果启用了 Saaswedo 端的连接，但未启用 Intune 端的连接，Intune 会忽略接收到的通信。

以下 Graph 资源可用于在 Intune 中管理电信费用：  

- [设备管理](intune-tem-devicemanagement.md)
- [电信费用管理合作伙伴](intune-tem-telecomexpensemanagementpartner.md)






