---
title: managedAppNotificationRestriction 枚举类型
description: 限制托管应用程序通知
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e89f9b17ae7a94a9d7447d802821047cdfc09f28
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42781822"
---
# <a name="managedappnotificationrestriction-enum-type"></a><span data-ttu-id="ea000-103">managedAppNotificationRestriction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ea000-103">managedAppNotificationRestriction enum type</span></span>

> <span data-ttu-id="ea000-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ea000-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea000-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ea000-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea000-106">限制托管应用程序通知</span><span class="sxs-lookup"><span data-stu-id="ea000-106">Restrict managed app notification</span></span>

## <a name="members"></a><span data-ttu-id="ea000-107">成员</span><span class="sxs-lookup"><span data-stu-id="ea000-107">Members</span></span>
|<span data-ttu-id="ea000-108">成员</span><span class="sxs-lookup"><span data-stu-id="ea000-108">Member</span></span>|<span data-ttu-id="ea000-109">值</span><span class="sxs-lookup"><span data-stu-id="ea000-109">Value</span></span>|<span data-ttu-id="ea000-110">说明</span><span class="sxs-lookup"><span data-stu-id="ea000-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea000-111">允许</span><span class="sxs-lookup"><span data-stu-id="ea000-111">allow</span></span>|<span data-ttu-id="ea000-112">0</span><span class="sxs-lookup"><span data-stu-id="ea000-112">0</span></span>|<span data-ttu-id="ea000-113">共享所有通知。</span><span class="sxs-lookup"><span data-stu-id="ea000-113">Share all notifications.</span></span>|
|<span data-ttu-id="ea000-114">blockOrganizationalData</span><span class="sxs-lookup"><span data-stu-id="ea000-114">blockOrganizationalData</span></span>|<span data-ttu-id="ea000-115">1</span><span class="sxs-lookup"><span data-stu-id="ea000-115">1</span></span>|<span data-ttu-id="ea000-116">不要在通知中共享 Orgnizational 数据。</span><span class="sxs-lookup"><span data-stu-id="ea000-116">Do not share Orgnizational data in notifications.</span></span>|
|<span data-ttu-id="ea000-117">数据</span><span class="sxs-lookup"><span data-stu-id="ea000-117">block</span></span>|<span data-ttu-id="ea000-118">双面</span><span class="sxs-lookup"><span data-stu-id="ea000-118">2</span></span>|<span data-ttu-id="ea000-119">不共享通知。</span><span class="sxs-lookup"><span data-stu-id="ea000-119">Do not share notifications.</span></span>|



