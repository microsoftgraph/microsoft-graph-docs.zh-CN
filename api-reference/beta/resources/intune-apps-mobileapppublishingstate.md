---
title: mobileAppPublishingState 枚举类型
description: 指示应用程序的发布状态。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 24a17e63570d46a1fd1771bf25e5bd0d397f9088
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890984"
---
# <a name="mobileapppublishingstate-enum-type"></a><span data-ttu-id="1b0d7-103">mobileAppPublishingState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1b0d7-103">mobileAppPublishingState enum type</span></span>

> <span data-ttu-id="1b0d7-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1b0d7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1b0d7-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1b0d7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1b0d7-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1b0d7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1b0d7-107">指示应用程序的发布状态。</span><span class="sxs-lookup"><span data-stu-id="1b0d7-107">Indicates the publishing state of an app.</span></span>
## <a name="members"></a><span data-ttu-id="1b0d7-108">成员</span><span class="sxs-lookup"><span data-stu-id="1b0d7-108">Members</span></span>
|<span data-ttu-id="1b0d7-109">成员</span><span class="sxs-lookup"><span data-stu-id="1b0d7-109">Member</span></span>|<span data-ttu-id="1b0d7-110">值</span><span class="sxs-lookup"><span data-stu-id="1b0d7-110">Value</span></span>|<span data-ttu-id="1b0d7-111">Description</span><span class="sxs-lookup"><span data-stu-id="1b0d7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b0d7-112">notPublished</span><span class="sxs-lookup"><span data-stu-id="1b0d7-112">notPublished</span></span>|<span data-ttu-id="1b0d7-113">0</span><span class="sxs-lookup"><span data-stu-id="1b0d7-113">0</span></span>|<span data-ttu-id="1b0d7-114">尚未发布应用程序。</span><span class="sxs-lookup"><span data-stu-id="1b0d7-114">The app is not yet published.</span></span>|
|<span data-ttu-id="1b0d7-115">处理</span><span class="sxs-lookup"><span data-stu-id="1b0d7-115">processing</span></span>|<span data-ttu-id="1b0d7-116">1</span><span class="sxs-lookup"><span data-stu-id="1b0d7-116">1</span></span>|<span data-ttu-id="1b0d7-117">待处理的服务商处理应用程序。</span><span class="sxs-lookup"><span data-stu-id="1b0d7-117">The app is pending service-side processing.</span></span>|
|<span data-ttu-id="1b0d7-118">已发布</span><span class="sxs-lookup"><span data-stu-id="1b0d7-118">published</span></span>|<span data-ttu-id="1b0d7-119">2</span><span class="sxs-lookup"><span data-stu-id="1b0d7-119">2</span></span>|<span data-ttu-id="1b0d7-120">发布应用程序。</span><span class="sxs-lookup"><span data-stu-id="1b0d7-120">The app is published.</span></span>|





