---
title: mobileAppPublishingState 枚举类型
description: 指示应用程序的发布状态。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: db10e62e714e50ccdf9bac933b2746cb52ea25eb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423879"
---
# <a name="mobileapppublishingstate-enum-type"></a><span data-ttu-id="7055e-103">mobileAppPublishingState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="7055e-103">mobileAppPublishingState enum type</span></span>

> <span data-ttu-id="7055e-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="7055e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7055e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7055e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7055e-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7055e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7055e-107">指示应用程序的发布状态。</span><span class="sxs-lookup"><span data-stu-id="7055e-107">Indicates the publishing state of an app.</span></span>

## <a name="members"></a><span data-ttu-id="7055e-108">成员</span><span class="sxs-lookup"><span data-stu-id="7055e-108">Members</span></span>
|<span data-ttu-id="7055e-109">成员</span><span class="sxs-lookup"><span data-stu-id="7055e-109">Member</span></span>|<span data-ttu-id="7055e-110">值</span><span class="sxs-lookup"><span data-stu-id="7055e-110">Value</span></span>|<span data-ttu-id="7055e-111">说明</span><span class="sxs-lookup"><span data-stu-id="7055e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7055e-112">notPublished</span><span class="sxs-lookup"><span data-stu-id="7055e-112">notPublished</span></span>|<span data-ttu-id="7055e-113">0</span><span class="sxs-lookup"><span data-stu-id="7055e-113">0</span></span>|<span data-ttu-id="7055e-114">尚未发布应用程序。</span><span class="sxs-lookup"><span data-stu-id="7055e-114">The app is not yet published.</span></span>|
|<span data-ttu-id="7055e-115">处理</span><span class="sxs-lookup"><span data-stu-id="7055e-115">processing</span></span>|<span data-ttu-id="7055e-116">1</span><span class="sxs-lookup"><span data-stu-id="7055e-116">1</span></span>|<span data-ttu-id="7055e-117">待处理的服务商处理应用程序。</span><span class="sxs-lookup"><span data-stu-id="7055e-117">The app is pending service-side processing.</span></span>|
|<span data-ttu-id="7055e-118">已发布</span><span class="sxs-lookup"><span data-stu-id="7055e-118">published</span></span>|<span data-ttu-id="7055e-119">2</span><span class="sxs-lookup"><span data-stu-id="7055e-119">2</span></span>|<span data-ttu-id="7055e-120">发布应用程序。</span><span class="sxs-lookup"><span data-stu-id="7055e-120">The app is published.</span></span>|




