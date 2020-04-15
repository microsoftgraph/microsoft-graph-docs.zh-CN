---
title: mobileAppPublishingState 枚举类型
description: 指示应用程序的发布状态。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7e15365bbb450bbb65d585f7c6790b9585e88ae6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439657"
---
# <a name="mobileapppublishingstate-enum-type"></a><span data-ttu-id="4c08a-103">mobileAppPublishingState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4c08a-103">mobileAppPublishingState enum type</span></span>

<span data-ttu-id="4c08a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c08a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4c08a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4c08a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c08a-106">指示应用程序的发布状态。</span><span class="sxs-lookup"><span data-stu-id="4c08a-106">Indicates the publishing state of an app.</span></span>

## <a name="members"></a><span data-ttu-id="4c08a-107">成员</span><span class="sxs-lookup"><span data-stu-id="4c08a-107">Members</span></span>
|<span data-ttu-id="4c08a-108">成员</span><span class="sxs-lookup"><span data-stu-id="4c08a-108">Member</span></span>|<span data-ttu-id="4c08a-109">值</span><span class="sxs-lookup"><span data-stu-id="4c08a-109">Value</span></span>|<span data-ttu-id="4c08a-110">说明</span><span class="sxs-lookup"><span data-stu-id="4c08a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c08a-111">notPublished</span><span class="sxs-lookup"><span data-stu-id="4c08a-111">notPublished</span></span>|<span data-ttu-id="4c08a-112">0</span><span class="sxs-lookup"><span data-stu-id="4c08a-112">0</span></span>|<span data-ttu-id="4c08a-113">应用尚未发布。</span><span class="sxs-lookup"><span data-stu-id="4c08a-113">The app is not yet published.</span></span>|
|<span data-ttu-id="4c08a-114">处理</span><span class="sxs-lookup"><span data-stu-id="4c08a-114">processing</span></span>|<span data-ttu-id="4c08a-115">1</span><span class="sxs-lookup"><span data-stu-id="4c08a-115">1</span></span>|<span data-ttu-id="4c08a-116">应用程序正在等待服务端处理。</span><span class="sxs-lookup"><span data-stu-id="4c08a-116">The app is pending service-side processing.</span></span>|
|<span data-ttu-id="4c08a-117">发布</span><span class="sxs-lookup"><span data-stu-id="4c08a-117">published</span></span>|<span data-ttu-id="4c08a-118">双面</span><span class="sxs-lookup"><span data-stu-id="4c08a-118">2</span></span>|<span data-ttu-id="4c08a-119">应用程序已发布。</span><span class="sxs-lookup"><span data-stu-id="4c08a-119">The app is published.</span></span>|







