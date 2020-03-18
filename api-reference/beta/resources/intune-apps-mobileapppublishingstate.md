---
title: mobileAppPublishingState 枚举类型
description: 指示应用程序的发布状态。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d82f2c4ab2a486e5d85369b8ae67e9b1e74b5324
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797788"
---
# <a name="mobileapppublishingstate-enum-type"></a><span data-ttu-id="25b85-103">mobileAppPublishingState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="25b85-103">mobileAppPublishingState enum type</span></span>

> <span data-ttu-id="25b85-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="25b85-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25b85-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="25b85-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25b85-106">指示应用程序的发布状态。</span><span class="sxs-lookup"><span data-stu-id="25b85-106">Indicates the publishing state of an app.</span></span>

## <a name="members"></a><span data-ttu-id="25b85-107">成员</span><span class="sxs-lookup"><span data-stu-id="25b85-107">Members</span></span>
|<span data-ttu-id="25b85-108">成员</span><span class="sxs-lookup"><span data-stu-id="25b85-108">Member</span></span>|<span data-ttu-id="25b85-109">值</span><span class="sxs-lookup"><span data-stu-id="25b85-109">Value</span></span>|<span data-ttu-id="25b85-110">说明</span><span class="sxs-lookup"><span data-stu-id="25b85-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25b85-111">notPublished</span><span class="sxs-lookup"><span data-stu-id="25b85-111">notPublished</span></span>|<span data-ttu-id="25b85-112">0</span><span class="sxs-lookup"><span data-stu-id="25b85-112">0</span></span>|<span data-ttu-id="25b85-113">应用尚未发布。</span><span class="sxs-lookup"><span data-stu-id="25b85-113">The app is not yet published.</span></span>|
|<span data-ttu-id="25b85-114">处理</span><span class="sxs-lookup"><span data-stu-id="25b85-114">processing</span></span>|<span data-ttu-id="25b85-115">1</span><span class="sxs-lookup"><span data-stu-id="25b85-115">1</span></span>|<span data-ttu-id="25b85-116">应用程序正在等待服务端处理。</span><span class="sxs-lookup"><span data-stu-id="25b85-116">The app is pending service-side processing.</span></span>|
|<span data-ttu-id="25b85-117">发布</span><span class="sxs-lookup"><span data-stu-id="25b85-117">published</span></span>|<span data-ttu-id="25b85-118">双面</span><span class="sxs-lookup"><span data-stu-id="25b85-118">2</span></span>|<span data-ttu-id="25b85-119">应用程序已发布。</span><span class="sxs-lookup"><span data-stu-id="25b85-119">The app is published.</span></span>|



