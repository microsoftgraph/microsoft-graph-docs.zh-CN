---
title: 呼叫记录概述
description: 呼叫记录可帮助您深入了解组织内发生的呼叫和会议。
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 11ca92e183531e133f5df20ec6a0d0e935487322
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601445"
---
# <a name="call-records-overview"></a><span data-ttu-id="b8efe-103">呼叫记录概述</span><span class="sxs-lookup"><span data-stu-id="b8efe-103">Call records overview</span></span>

<span data-ttu-id="b8efe-104">通话记录提供了使用 Microsoft Teams 或 Skype for Business 时组织内发生的通话和联机会议的使用情况和诊断信息。</span><span class="sxs-lookup"><span data-stu-id="b8efe-104">Call records provide usage and diagnostic information about the calls and online meetings that occur within your organization when using Microsoft Teams or Skype for Business.</span></span> <span data-ttu-id="b8efe-105">可以使用使用率和诊断数据来为您的企业生成自定义报告，以帮助监控采用或解决呼叫质量问题。</span><span class="sxs-lookup"><span data-stu-id="b8efe-105">Usage and diagnostic data can be consumed to produce custom reporting for your business to help monitor adoption or to troubleshoot call quality issues.</span></span>

<span data-ttu-id="b8efe-106">组织可以使用 Microsoft Graph [webhook 订阅](/graph/api/resources/webhooks?view=graph-rest-1.0) 功能订阅对呼叫记录所做的更改，从而允许他们生成来自数据的近实时报告或在某些情况下（如紧急呼叫）发出警报。</span><span class="sxs-lookup"><span data-stu-id="b8efe-106">Organizations can subscribe to changes to call records using the Microsoft Graph [webhook subscriptions](/graph/api/resources/webhooks?view=graph-rest-1.0) capability, allowing them to build near-real-time reports from the data or to alert on certain scenarios like emergency calls.</span></span>

> <span data-ttu-id="b8efe-107">**重要说明：** 授予对应用程序的 CallRecords 权限时，请务必谨慎。</span><span class="sxs-lookup"><span data-stu-id="b8efe-107">**Important:** Use discretion when granting the CallRecords.Read.All permission to applications.</span></span> <span data-ttu-id="b8efe-108">呼叫记录可提供业务运营的见解，因此可以成为恶意参与者的目标。</span><span class="sxs-lookup"><span data-stu-id="b8efe-108">Call records can provide insights into the operation of your business, and therefore can be a target for malicious actors.</span></span> <span data-ttu-id="b8efe-109">仅为你信任的应用程序授予此权限，以满足你的数据保护要求。</span><span class="sxs-lookup"><span data-stu-id="b8efe-109">Only grant this permission to applications you trust to meet your data protection requirements.</span></span>

## <a name="subscribe-to-call-records"></a><span data-ttu-id="b8efe-110">订阅呼叫记录</span><span class="sxs-lookup"><span data-stu-id="b8efe-110">Subscribe to call records</span></span>

<span data-ttu-id="b8efe-111">组织和合作伙伴通常拥有自己的工具来生成有关呼叫和联机会议的报告。</span><span class="sxs-lookup"><span data-stu-id="b8efe-111">Organizations and partners often have their own tooling for generating reports about calls and online meetings.</span></span> <span data-ttu-id="b8efe-112">使用 webhook，他们可以在创建呼叫记录时接收连续的呼叫记录源。</span><span class="sxs-lookup"><span data-stu-id="b8efe-112">Using webhooks, they can receive a continuous feed of call records as they are created.</span></span> <span data-ttu-id="b8efe-113">此推送模型使组织和合作伙伴能够构建自己的实时报告解决方案。</span><span class="sxs-lookup"><span data-stu-id="b8efe-113">This push-model enables organizations and partners to build their own real-time reporting solutions.</span></span>

## <a name="look-up-a-call-record-by-its-call-id"></a><span data-ttu-id="b8efe-114">按呼叫 ID 查找呼叫记录</span><span class="sxs-lookup"><span data-stu-id="b8efe-114">Look up a call record by its call ID</span></span>

<span data-ttu-id="b8efe-115">应用程序可以按其 ID 检索 [呼叫记录](/graph/api/resources/callrecords-callrecord?view=graph-rest-1.0) 。</span><span class="sxs-lookup"><span data-stu-id="b8efe-115">Applications can retrieve a [call record](/graph/api/resources/callrecords-callrecord?view=graph-rest-1.0) by its ID.</span></span> <span data-ttu-id="b8efe-116">可以从 webhook 通知或从管理工具检索到此 ID。</span><span class="sxs-lookup"><span data-stu-id="b8efe-116">This ID can be determined from a webhook notification or retrieved from administrative tools.</span></span>

## <a name="get-call-record-reports"></a><span data-ttu-id="b8efe-117">获取呼叫记录报告</span><span class="sxs-lookup"><span data-stu-id="b8efe-117">Get call record reports</span></span>

<span data-ttu-id="b8efe-118">使用 Microsoft 团队连接到公共交换电话网络 (PSTN) 的组织通常需要跟踪此使用情况，以了解相关的成本。</span><span class="sxs-lookup"><span data-stu-id="b8efe-118">Organizations that use Microsoft Teams to connect to the public switched telephone network (PSTN) usually want to track this usage to understand the associated costs.</span></span> <span data-ttu-id="b8efe-119">[GetPstnCalls](/graph/api/callrecords-callrecord-getpstncalls?view=graph-rest-beta)和[getDirectRoutingCalls](/graph/api/callrecords-callrecord-getdirectroutingcalls?view=graph-rest-beta)函数以表格格式返回[呼叫记录](/graph/api/resources/callrecords-callrecord?view=graph-rest-beta)数据的投影。</span><span class="sxs-lookup"><span data-stu-id="b8efe-119">The [getPstnCalls](/graph/api/callrecords-callrecord-getpstncalls?view=graph-rest-beta) and [getDirectRoutingCalls](/graph/api/callrecords-callrecord-getdirectroutingcalls?view=graph-rest-beta) functions return a projection of [call record](/graph/api/resources/callrecords-callrecord?view=graph-rest-beta) data in a tabular format.</span></span>

## <a name="see-also"></a><span data-ttu-id="b8efe-120">另请参阅</span><span class="sxs-lookup"><span data-stu-id="b8efe-120">See also</span></span>

- [<span data-ttu-id="b8efe-121">通话记录权限</span><span class="sxs-lookup"><span data-stu-id="b8efe-121">Call records permissions</span></span>](./permissions-reference.md#call-records-permissions)