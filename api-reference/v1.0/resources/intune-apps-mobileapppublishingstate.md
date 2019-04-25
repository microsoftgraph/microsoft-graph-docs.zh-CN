---
title: mobileAppPublishingState 枚举类型
description: 指示应用程序的发布状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b0823576dd1792b01193d600cdebbe171b47052
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32557836"
---
# <a name="mobileapppublishingstate-enum-type"></a><span data-ttu-id="61132-103">mobileAppPublishingState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="61132-103">mobileAppPublishingState enum type</span></span>

> <span data-ttu-id="61132-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="61132-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61132-105">指示应用程序的发布状态。</span><span class="sxs-lookup"><span data-stu-id="61132-105">Indicates the publishing state of an app.</span></span>

## <a name="members"></a><span data-ttu-id="61132-106">成员</span><span class="sxs-lookup"><span data-stu-id="61132-106">Members</span></span>
|<span data-ttu-id="61132-107">成员</span><span class="sxs-lookup"><span data-stu-id="61132-107">Member</span></span>|<span data-ttu-id="61132-108">值</span><span class="sxs-lookup"><span data-stu-id="61132-108">Value</span></span>|<span data-ttu-id="61132-109">说明</span><span class="sxs-lookup"><span data-stu-id="61132-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61132-110">notPublished</span><span class="sxs-lookup"><span data-stu-id="61132-110">notPublished</span></span>|<span data-ttu-id="61132-111">0</span><span class="sxs-lookup"><span data-stu-id="61132-111">0</span></span>|<span data-ttu-id="61132-112">应用尚未发布。</span><span class="sxs-lookup"><span data-stu-id="61132-112">The app is not yet published.</span></span>|
|<span data-ttu-id="61132-113">处理</span><span class="sxs-lookup"><span data-stu-id="61132-113">processing</span></span>|<span data-ttu-id="61132-114">1</span><span class="sxs-lookup"><span data-stu-id="61132-114">1</span></span>|<span data-ttu-id="61132-115">应用程序正在等待服务端处理。</span><span class="sxs-lookup"><span data-stu-id="61132-115">The app is pending service-side processing.</span></span>|
|<span data-ttu-id="61132-116">发布</span><span class="sxs-lookup"><span data-stu-id="61132-116">published</span></span>|<span data-ttu-id="61132-117">2 </span><span class="sxs-lookup"><span data-stu-id="61132-117">2</span></span>|<span data-ttu-id="61132-118">应用程序已发布。</span><span class="sxs-lookup"><span data-stu-id="61132-118">The app is published.</span></span>|



