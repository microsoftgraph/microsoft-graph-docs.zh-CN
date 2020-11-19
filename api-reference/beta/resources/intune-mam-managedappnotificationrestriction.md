---
title: managedAppNotificationRestriction 枚举类型
description: 限制托管应用程序通知
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f925830d1608718612755841f1fad7d41fa50874
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49207272"
---
# <a name="managedappnotificationrestriction-enum-type"></a><span data-ttu-id="c0d4e-103">managedAppNotificationRestriction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c0d4e-103">managedAppNotificationRestriction enum type</span></span>

<span data-ttu-id="c0d4e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0d4e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0d4e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c0d4e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0d4e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c0d4e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0d4e-107">限制托管应用程序通知</span><span class="sxs-lookup"><span data-stu-id="c0d4e-107">Restrict managed app notification</span></span>

## <a name="members"></a><span data-ttu-id="c0d4e-108">成员</span><span class="sxs-lookup"><span data-stu-id="c0d4e-108">Members</span></span>
|<span data-ttu-id="c0d4e-109">成员</span><span class="sxs-lookup"><span data-stu-id="c0d4e-109">Member</span></span>|<span data-ttu-id="c0d4e-110">值</span><span class="sxs-lookup"><span data-stu-id="c0d4e-110">Value</span></span>|<span data-ttu-id="c0d4e-111">说明</span><span class="sxs-lookup"><span data-stu-id="c0d4e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0d4e-112">允许</span><span class="sxs-lookup"><span data-stu-id="c0d4e-112">allow</span></span>|<span data-ttu-id="c0d4e-113">0</span><span class="sxs-lookup"><span data-stu-id="c0d4e-113">0</span></span>|<span data-ttu-id="c0d4e-114">共享所有通知。</span><span class="sxs-lookup"><span data-stu-id="c0d4e-114">Share all notifications.</span></span>|
|<span data-ttu-id="c0d4e-115">blockOrganizationalData</span><span class="sxs-lookup"><span data-stu-id="c0d4e-115">blockOrganizationalData</span></span>|<span data-ttu-id="c0d4e-116">1</span><span class="sxs-lookup"><span data-stu-id="c0d4e-116">1</span></span>|<span data-ttu-id="c0d4e-117">不要在通知中共享 Orgnizational 数据。</span><span class="sxs-lookup"><span data-stu-id="c0d4e-117">Do not share Orgnizational data in notifications.</span></span>|
|<span data-ttu-id="c0d4e-118">数据</span><span class="sxs-lookup"><span data-stu-id="c0d4e-118">block</span></span>|<span data-ttu-id="c0d4e-119">双面</span><span class="sxs-lookup"><span data-stu-id="c0d4e-119">2</span></span>|<span data-ttu-id="c0d4e-120">不共享通知。</span><span class="sxs-lookup"><span data-stu-id="c0d4e-120">Do not share notifications.</span></span>|




