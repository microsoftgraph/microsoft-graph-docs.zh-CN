---
title: managedAppNotificationRestriction 枚举类型
description: 限制托管应用程序通知
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 78d031f4aa7b7aef5c154cc1d485fd71753855b8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332097"
---
# <a name="managedappnotificationrestriction-enum-type"></a><span data-ttu-id="01da9-103">managedAppNotificationRestriction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="01da9-103">managedAppNotificationRestriction enum type</span></span>

> <span data-ttu-id="01da9-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="01da9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01da9-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="01da9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01da9-106">限制托管应用程序通知</span><span class="sxs-lookup"><span data-stu-id="01da9-106">Restrict managed app notification</span></span>

## <a name="members"></a><span data-ttu-id="01da9-107">成员</span><span class="sxs-lookup"><span data-stu-id="01da9-107">Members</span></span>
|<span data-ttu-id="01da9-108">成员</span><span class="sxs-lookup"><span data-stu-id="01da9-108">Member</span></span>|<span data-ttu-id="01da9-109">值</span><span class="sxs-lookup"><span data-stu-id="01da9-109">Value</span></span>|<span data-ttu-id="01da9-110">说明</span><span class="sxs-lookup"><span data-stu-id="01da9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01da9-111">允许</span><span class="sxs-lookup"><span data-stu-id="01da9-111">allow</span></span>|<span data-ttu-id="01da9-112">0</span><span class="sxs-lookup"><span data-stu-id="01da9-112">0</span></span>|<span data-ttu-id="01da9-113">共享所有通知。</span><span class="sxs-lookup"><span data-stu-id="01da9-113">Share all notifications.</span></span>|
|<span data-ttu-id="01da9-114">blockOrganizationalData</span><span class="sxs-lookup"><span data-stu-id="01da9-114">blockOrganizationalData</span></span>|<span data-ttu-id="01da9-115">1</span><span class="sxs-lookup"><span data-stu-id="01da9-115">1</span></span>|<span data-ttu-id="01da9-116">不要在通知中共享 Orgnizational 数据。</span><span class="sxs-lookup"><span data-stu-id="01da9-116">Do not share Orgnizational data in notifications.</span></span>|
|<span data-ttu-id="01da9-117">数据</span><span class="sxs-lookup"><span data-stu-id="01da9-117">block</span></span>|<span data-ttu-id="01da9-118">双面</span><span class="sxs-lookup"><span data-stu-id="01da9-118">2</span></span>|<span data-ttu-id="01da9-119">不共享通知。</span><span class="sxs-lookup"><span data-stu-id="01da9-119">Do not share notifications.</span></span>|



