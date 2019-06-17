---
title: Microsoft Intune 中的电信费用管理-Microsoft Graph API
description: 列出与租户组织的电信费用管理相关的适用于 Intune 终结点 (REST) 的 Microsoft Graph API。
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: cd63fcc46cc7afef661ebe611194fc3181e7d15c
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34988207"
---
# <a name="telecom-expense-management-in-microsoft-intune"></a><span data-ttu-id="1b5e0-103">Microsoft Intune 中的电信费用管理</span><span class="sxs-lookup"><span data-stu-id="1b5e0-103">Telecom expense management in Microsoft Intune</span></span>

> <span data-ttu-id="1b5e0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1b5e0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1b5e0-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1b5e0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1b5e0-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1b5e0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b5e0-107">使用 Saaswedo 电信费用管理服务时，你可以在企业拥有的设备上限制数据使用和漫游，它会与 Intune 集成。</span><span class="sxs-lookup"><span data-stu-id="1b5e0-107">You can limit data usage and roaming on corporate-owned devices when you use the Saaswedo telecom expense management service, which integrates with Intune.</span></span> <span data-ttu-id="1b5e0-108">该服务让你可以设置和强制执行使用限制，并在超过配置的阈值时向用户发送警报。</span><span class="sxs-lookup"><span data-stu-id="1b5e0-108">The service enables you to set and enforce usage limits and to send users an alert when they exceed a configured threshold.</span></span> <span data-ttu-id="1b5e0-109">用户超过阈值时，你还可以配置服务以采取其他操作，例如禁用漫游。</span><span class="sxs-lookup"><span data-stu-id="1b5e0-109">You can also configure the service to take different actions, such as disabling roaming, when users exceed the threshold.</span></span> <span data-ttu-id="1b5e0-110">Saaswedo 控制台中提供包含数据使用情况和监视信息的报告。</span><span class="sxs-lookup"><span data-stu-id="1b5e0-110">Reports that provide data usage and monitoring information are available in the Saaswedo console.</span></span> <span data-ttu-id="1b5e0-111">通过 Intune 使用 Saaswedo 电信费用管理服务之前，你需要在 Saaswedo 控制台和 Intune 中配置设置。</span><span class="sxs-lookup"><span data-stu-id="1b5e0-111">Before you can use the Saaswedo telecom expense management service with Intune, you need to configure settings in a Saaswedo console and in Intune.</span></span> <span data-ttu-id="1b5e0-112">必须打开 Saaswedo 服务和 Intune 的连接。</span><span class="sxs-lookup"><span data-stu-id="1b5e0-112">The connection must be turned on for the Saaswedo service and for Intune.</span></span> <span data-ttu-id="1b5e0-113">如果启用了 Saaswedo 端的连接，但未启用 Intune 端的连接，Intune 会忽略接收到的通信。</span><span class="sxs-lookup"><span data-stu-id="1b5e0-113">If the Saaswedo side of the connection is enabled, but not the Intune side, Intune receives the communication, but ignores it.</span></span>

<span data-ttu-id="1b5e0-114">以下 Graph 资源可用于在 Intune 中管理电信费用：</span><span class="sxs-lookup"><span data-stu-id="1b5e0-114">The following Graph resources are available to manage telecom expenses in Intune:</span></span>

- [<span data-ttu-id="1b5e0-115">电信费用管理合作伙伴</span><span class="sxs-lookup"><span data-stu-id="1b5e0-115">Telecom expense management partner</span></span>](intune-tem-telecomexpensemanagementpartner.md)
