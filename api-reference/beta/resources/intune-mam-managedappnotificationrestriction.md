---
title: managedAppNotificationRestriction 枚举类型
description: 限制托管应用程序通知
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 941fcac27234996e78c67a572fe0a2bbe66f10f0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527911"
---
# <a name="managedappnotificationrestriction-enum-type"></a><span data-ttu-id="a1a0c-103">managedAppNotificationRestriction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a1a0c-103">managedAppNotificationRestriction enum type</span></span>

<span data-ttu-id="a1a0c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="a1a0c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a1a0c-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a1a0c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1a0c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a1a0c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1a0c-107">限制托管应用程序通知</span><span class="sxs-lookup"><span data-stu-id="a1a0c-107">Restrict managed app notification</span></span>

## <a name="members"></a><span data-ttu-id="a1a0c-108">成员</span><span class="sxs-lookup"><span data-stu-id="a1a0c-108">Members</span></span>
|<span data-ttu-id="a1a0c-109">成员</span><span class="sxs-lookup"><span data-stu-id="a1a0c-109">Member</span></span>|<span data-ttu-id="a1a0c-110">值</span><span class="sxs-lookup"><span data-stu-id="a1a0c-110">Value</span></span>|<span data-ttu-id="a1a0c-111">说明</span><span class="sxs-lookup"><span data-stu-id="a1a0c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1a0c-112">允许</span><span class="sxs-lookup"><span data-stu-id="a1a0c-112">allow</span></span>|<span data-ttu-id="a1a0c-113">0</span><span class="sxs-lookup"><span data-stu-id="a1a0c-113">0</span></span>|<span data-ttu-id="a1a0c-114">共享所有通知。</span><span class="sxs-lookup"><span data-stu-id="a1a0c-114">Share all notifications.</span></span>|
|<span data-ttu-id="a1a0c-115">blockOrganizationalData</span><span class="sxs-lookup"><span data-stu-id="a1a0c-115">blockOrganizationalData</span></span>|<span data-ttu-id="a1a0c-116">1 </span><span class="sxs-lookup"><span data-stu-id="a1a0c-116">1</span></span>|<span data-ttu-id="a1a0c-117">不要在通知中共享 Orgnizational 数据。</span><span class="sxs-lookup"><span data-stu-id="a1a0c-117">Do not share Orgnizational data in notifications.</span></span>|
|<span data-ttu-id="a1a0c-118">数据</span><span class="sxs-lookup"><span data-stu-id="a1a0c-118">block</span></span>|<span data-ttu-id="a1a0c-119">2 </span><span class="sxs-lookup"><span data-stu-id="a1a0c-119">2</span></span>|<span data-ttu-id="a1a0c-120">不共享通知。</span><span class="sxs-lookup"><span data-stu-id="a1a0c-120">Do not share notifications.</span></span>|



