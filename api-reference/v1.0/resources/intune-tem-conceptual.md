---
title: Microsoft Intune 中的电信费用管理
description: 使用 Saaswedo 电信费用管理服务时，你可以在企业拥有的设备上限制数据使用和漫游，它会与 Intune 集成。 该服务让你可以设置和强制执行使用限制，并在超过配置的阈值时向用户发送警报。 用户超过阈值时，你还可以配置服务以采取其他操作，例如禁用漫游。 Saaswedo 控制台中提供包含数据使用情况和监视信息的报告。 通过 Intune 使用 Saaswedo 电信费用管理服务之前，你需要在 Saaswedo 控制台和 Intune 中配置设置。 必须打开 Saaswedo 服务和 Intune 的连接。 如果启用了 Saaswedo 端的连接，但未启用 Intune 端的连接，Intune 会忽略接收到的通信。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 7a23f44192b17ae2dfa745496dfbc2b4b1f5a836
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732373"
---
# <a name="telecom-expense-management-in-microsoft-intune"></a><span data-ttu-id="b8855-109">Microsoft Intune 中的电信费用管理</span><span class="sxs-lookup"><span data-stu-id="b8855-109">Telecom expense management in Microsoft Intune</span></span>

<span data-ttu-id="b8855-110">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8855-110">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b8855-111">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户 [正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b8855-111">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="b8855-112">使用 Saaswedo 电信费用管理服务时，你可以在企业拥有的设备上限制数据使用和漫游，它会与 Intune 集成。</span><span class="sxs-lookup"><span data-stu-id="b8855-112">You can limit data usage and roaming on corporate-owned devices when you use the Saaswedo telecom expense management service, which integrates with Intune.</span></span> <span data-ttu-id="b8855-113">该服务让你可以设置和强制执行使用限制，并在超过配置的阈值时向用户发送警报。</span><span class="sxs-lookup"><span data-stu-id="b8855-113">The service enables you to set and enforce usage limits and to send users an alert when they exceed a configured threshold.</span></span> <span data-ttu-id="b8855-114">用户超过阈值时，你还可以配置服务以采取其他操作，例如禁用漫游。</span><span class="sxs-lookup"><span data-stu-id="b8855-114">You can also configure the service to take different actions, such as disabling roaming, when users exceed the threshold.</span></span> <span data-ttu-id="b8855-115">Saaswedo 控制台中提供包含数据使用情况和监视信息的报告。</span><span class="sxs-lookup"><span data-stu-id="b8855-115">Reports that provide data usage and monitoring information are available in the Saaswedo console.</span></span> <span data-ttu-id="b8855-116">通过 Intune 使用 Saaswedo 电信费用管理服务之前，你需要在 Saaswedo 控制台和 Intune 中配置设置。</span><span class="sxs-lookup"><span data-stu-id="b8855-116">Before you can use the Saaswedo telecom expense management service with Intune, you need to configure settings in a Saaswedo console and in Intune.</span></span> <span data-ttu-id="b8855-117">必须打开 Saaswedo 服务和 Intune 的连接。</span><span class="sxs-lookup"><span data-stu-id="b8855-117">The connection must be turned on for the Saaswedo service and for Intune.</span></span> <span data-ttu-id="b8855-118">如果启用了 Saaswedo 端的连接，但未启用 Intune 端的连接，Intune 会忽略接收到的通信。</span><span class="sxs-lookup"><span data-stu-id="b8855-118">If the Saaswedo side of the connection is enabled, but not the Intune side, Intune receives the communication, but ignores it.</span></span>

<span data-ttu-id="b8855-119">以下 Graph 资源可用于在 Intune 中管理电信费用：</span><span class="sxs-lookup"><span data-stu-id="b8855-119">The following Graph resources are available to manage telecom expenses in Intune:</span></span>  

- [<span data-ttu-id="b8855-120">电信费用管理合作伙伴</span><span class="sxs-lookup"><span data-stu-id="b8855-120">Telecom expense management partner</span></span>](intune-tem-telecomexpensemanagementpartner.md)






