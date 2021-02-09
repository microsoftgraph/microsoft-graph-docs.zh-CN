---
title: Microsoft Intune 中的电信费用管理 - Microsoft Graph API
description: 列出适用于 Intune 终结点的 Microsoft Graph API (REST) 租户组织的电信费用管理相关。
localization_priority: Normal
author: dougeby
ms.prod: intune
ms.openlocfilehash: 471bd6315c35b713bb022cc9872f96ac70fcd050
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159470"
---
# <a name="telecom-expense-management-in-microsoft-intune"></a>Microsoft Intune 中的电信费用管理

命名空间：microsoft.graph

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

使用 Saaswedo 电信费用管理服务时，你可以在企业拥有的设备上限制数据使用和漫游，它会与 Intune 集成。 该服务让你可以设置和强制执行使用限制，并在超过配置的阈值时向用户发送警报。 用户超过阈值时，你还可以配置服务以采取其他操作，例如禁用漫游。 Saaswedo 控制台中提供包含数据使用情况和监视信息的报告。 通过 Intune 使用 Saaswedo 电信费用管理服务之前，你需要在 Saaswedo 控制台和 Intune 中配置设置。 必须打开 Saaswedo 服务和 Intune 的连接。 如果启用了 Saaswedo 端的连接，但未启用 Intune 端的连接，Intune 会忽略接收到的通信。

以下 Graph 资源可用于在 Intune 中管理电信费用：

- [电信费用管理合作伙伴](intune-tem-telecomexpensemanagementpartner.md)