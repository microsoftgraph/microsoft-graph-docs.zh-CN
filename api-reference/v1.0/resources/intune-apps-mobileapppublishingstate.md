---
title: mobileAppPublishingState 枚举类型
description: 指示应用程序的发布状态。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d00f9056a177715061edbff4332e86b925cf49ce
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532758"
---
# <a name="mobileapppublishingstate-enum-type"></a><span data-ttu-id="41775-103">mobileAppPublishingState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="41775-103">mobileAppPublishingState enum type</span></span>

<span data-ttu-id="41775-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41775-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="41775-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="41775-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41775-106">指示应用程序的发布状态。</span><span class="sxs-lookup"><span data-stu-id="41775-106">Indicates the publishing state of an app.</span></span>

## <a name="members"></a><span data-ttu-id="41775-107">成员</span><span class="sxs-lookup"><span data-stu-id="41775-107">Members</span></span>
|<span data-ttu-id="41775-108">成员</span><span class="sxs-lookup"><span data-stu-id="41775-108">Member</span></span>|<span data-ttu-id="41775-109">值</span><span class="sxs-lookup"><span data-stu-id="41775-109">Value</span></span>|<span data-ttu-id="41775-110">说明</span><span class="sxs-lookup"><span data-stu-id="41775-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41775-111">notPublished</span><span class="sxs-lookup"><span data-stu-id="41775-111">notPublished</span></span>|<span data-ttu-id="41775-112">0</span><span class="sxs-lookup"><span data-stu-id="41775-112">0</span></span>|<span data-ttu-id="41775-113">应用尚未发布。</span><span class="sxs-lookup"><span data-stu-id="41775-113">The app is not yet published.</span></span>|
|<span data-ttu-id="41775-114">处理</span><span class="sxs-lookup"><span data-stu-id="41775-114">processing</span></span>|<span data-ttu-id="41775-115">1 </span><span class="sxs-lookup"><span data-stu-id="41775-115">1</span></span>|<span data-ttu-id="41775-116">应用程序正在等待服务端处理。</span><span class="sxs-lookup"><span data-stu-id="41775-116">The app is pending service-side processing.</span></span>|
|<span data-ttu-id="41775-117">发布</span><span class="sxs-lookup"><span data-stu-id="41775-117">published</span></span>|<span data-ttu-id="41775-118">2 </span><span class="sxs-lookup"><span data-stu-id="41775-118">2</span></span>|<span data-ttu-id="41775-119">应用程序已发布。</span><span class="sxs-lookup"><span data-stu-id="41775-119">The app is published.</span></span>|




