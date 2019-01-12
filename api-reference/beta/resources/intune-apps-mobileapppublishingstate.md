---
title: mobileAppPublishingState 枚举类型
description: 指示应用程序的发布状态。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6b2ae893a0c971bfa0a80a09bb8e7c80b6146555
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932817"
---
# <a name="mobileapppublishingstate-enum-type"></a><span data-ttu-id="6a9c6-103">mobileAppPublishingState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6a9c6-103">mobileAppPublishingState enum type</span></span>

> <span data-ttu-id="6a9c6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6a9c6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a9c6-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6a9c6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6a9c6-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6a9c6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6a9c6-107">指示应用程序的发布状态。</span><span class="sxs-lookup"><span data-stu-id="6a9c6-107">Indicates the publishing state of an app.</span></span>
## <a name="members"></a><span data-ttu-id="6a9c6-108">成员</span><span class="sxs-lookup"><span data-stu-id="6a9c6-108">Members</span></span>
|<span data-ttu-id="6a9c6-109">成员</span><span class="sxs-lookup"><span data-stu-id="6a9c6-109">Member</span></span>|<span data-ttu-id="6a9c6-110">值</span><span class="sxs-lookup"><span data-stu-id="6a9c6-110">Value</span></span>|<span data-ttu-id="6a9c6-111">说明</span><span class="sxs-lookup"><span data-stu-id="6a9c6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a9c6-112">notPublished</span><span class="sxs-lookup"><span data-stu-id="6a9c6-112">notPublished</span></span>|<span data-ttu-id="6a9c6-113">0</span><span class="sxs-lookup"><span data-stu-id="6a9c6-113">0</span></span>|<span data-ttu-id="6a9c6-114">尚未发布应用程序。</span><span class="sxs-lookup"><span data-stu-id="6a9c6-114">The app is not yet published.</span></span>|
|<span data-ttu-id="6a9c6-115">处理</span><span class="sxs-lookup"><span data-stu-id="6a9c6-115">processing</span></span>|<span data-ttu-id="6a9c6-116">1</span><span class="sxs-lookup"><span data-stu-id="6a9c6-116">1</span></span>|<span data-ttu-id="6a9c6-117">待处理的服务商处理应用程序。</span><span class="sxs-lookup"><span data-stu-id="6a9c6-117">The app is pending service-side processing.</span></span>|
|<span data-ttu-id="6a9c6-118">已发布</span><span class="sxs-lookup"><span data-stu-id="6a9c6-118">published</span></span>|<span data-ttu-id="6a9c6-119">2</span><span class="sxs-lookup"><span data-stu-id="6a9c6-119">2</span></span>|<span data-ttu-id="6a9c6-120">发布应用程序。</span><span class="sxs-lookup"><span data-stu-id="6a9c6-120">The app is published.</span></span>|





