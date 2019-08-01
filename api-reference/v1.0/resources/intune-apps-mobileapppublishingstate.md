---
title: mobileAppPublishingState 枚举类型
description: 指示应用程序的发布状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 81361cabcd1ebade92e1c81b0c5a1677170473c4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032135"
---
# <a name="mobileapppublishingstate-enum-type"></a><span data-ttu-id="da18f-103">mobileAppPublishingState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="da18f-103">mobileAppPublishingState enum type</span></span>

> <span data-ttu-id="da18f-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="da18f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da18f-105">指示应用程序的发布状态。</span><span class="sxs-lookup"><span data-stu-id="da18f-105">Indicates the publishing state of an app.</span></span>

## <a name="members"></a><span data-ttu-id="da18f-106">成员</span><span class="sxs-lookup"><span data-stu-id="da18f-106">Members</span></span>
|<span data-ttu-id="da18f-107">成员</span><span class="sxs-lookup"><span data-stu-id="da18f-107">Member</span></span>|<span data-ttu-id="da18f-108">值</span><span class="sxs-lookup"><span data-stu-id="da18f-108">Value</span></span>|<span data-ttu-id="da18f-109">说明</span><span class="sxs-lookup"><span data-stu-id="da18f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da18f-110">notPublished</span><span class="sxs-lookup"><span data-stu-id="da18f-110">notPublished</span></span>|<span data-ttu-id="da18f-111">0</span><span class="sxs-lookup"><span data-stu-id="da18f-111">0</span></span>|<span data-ttu-id="da18f-112">应用尚未发布。</span><span class="sxs-lookup"><span data-stu-id="da18f-112">The app is not yet published.</span></span>|
|<span data-ttu-id="da18f-113">处理</span><span class="sxs-lookup"><span data-stu-id="da18f-113">processing</span></span>|<span data-ttu-id="da18f-114">1</span><span class="sxs-lookup"><span data-stu-id="da18f-114">1</span></span>|<span data-ttu-id="da18f-115">应用程序正在等待服务端处理。</span><span class="sxs-lookup"><span data-stu-id="da18f-115">The app is pending service-side processing.</span></span>|
|<span data-ttu-id="da18f-116">发布</span><span class="sxs-lookup"><span data-stu-id="da18f-116">published</span></span>|<span data-ttu-id="da18f-117">双面</span><span class="sxs-lookup"><span data-stu-id="da18f-117">2</span></span>|<span data-ttu-id="da18f-118">应用程序已发布。</span><span class="sxs-lookup"><span data-stu-id="da18f-118">The app is published.</span></span>|



