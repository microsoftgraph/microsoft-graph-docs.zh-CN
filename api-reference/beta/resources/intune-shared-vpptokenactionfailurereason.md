---
title: vppTokenActionFailureReason 枚举类型
description: 可能的 Apple 卷购买计划令牌操作失败的原因的类型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bba4c339b774fd32a852925729e2e158dc13e52d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393142"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="f5c7b-103">vppTokenActionFailureReason 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f5c7b-103">vppTokenActionFailureReason enum type</span></span>

> <span data-ttu-id="f5c7b-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="f5c7b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f5c7b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f5c7b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f5c7b-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f5c7b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5c7b-107">可能的 Apple 卷购买计划令牌操作失败的原因的类型。</span><span class="sxs-lookup"><span data-stu-id="f5c7b-107">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>

## <a name="members"></a><span data-ttu-id="f5c7b-108">成员</span><span class="sxs-lookup"><span data-stu-id="f5c7b-108">Members</span></span>
|<span data-ttu-id="f5c7b-109">成员</span><span class="sxs-lookup"><span data-stu-id="f5c7b-109">Member</span></span>|<span data-ttu-id="f5c7b-110">值</span><span class="sxs-lookup"><span data-stu-id="f5c7b-110">Value</span></span>|<span data-ttu-id="f5c7b-111">说明</span><span class="sxs-lookup"><span data-stu-id="f5c7b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5c7b-112">无</span><span class="sxs-lookup"><span data-stu-id="f5c7b-112">none</span></span>|<span data-ttu-id="f5c7b-113">0</span><span class="sxs-lookup"><span data-stu-id="f5c7b-113">0</span></span>|<span data-ttu-id="f5c7b-114">无。</span><span class="sxs-lookup"><span data-stu-id="f5c7b-114">None.</span></span>|
|<span data-ttu-id="f5c7b-115">appleFailure</span><span class="sxs-lookup"><span data-stu-id="f5c7b-115">appleFailure</span></span>|<span data-ttu-id="f5c7b-116">1</span><span class="sxs-lookup"><span data-stu-id="f5c7b-116">1</span></span>|<span data-ttu-id="f5c7b-117">在 Apple 的服务时出错。</span><span class="sxs-lookup"><span data-stu-id="f5c7b-117">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="f5c7b-118">internalError</span><span class="sxs-lookup"><span data-stu-id="f5c7b-118">internalError</span></span>|<span data-ttu-id="f5c7b-119">2</span><span class="sxs-lookup"><span data-stu-id="f5c7b-119">2</span></span>|<span data-ttu-id="f5c7b-120">存在内部错误。</span><span class="sxs-lookup"><span data-stu-id="f5c7b-120">There was an internal error.</span></span>|
|<span data-ttu-id="f5c7b-121">expiredVppToken</span><span class="sxs-lookup"><span data-stu-id="f5c7b-121">expiredVppToken</span></span>|<span data-ttu-id="f5c7b-122">3</span><span class="sxs-lookup"><span data-stu-id="f5c7b-122">3</span></span>|<span data-ttu-id="f5c7b-123">因为 Apple 卷购买计划令牌已过期时出错。</span><span class="sxs-lookup"><span data-stu-id="f5c7b-123">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="f5c7b-124">expiredApplePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="f5c7b-124">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="f5c7b-125">4</span><span class="sxs-lookup"><span data-stu-id="f5c7b-125">4</span></span>|<span data-ttu-id="f5c7b-126">由于 Apple 卷购买程序推送通知证书过期时出错。</span><span class="sxs-lookup"><span data-stu-id="f5c7b-126">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|




