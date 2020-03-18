---
title: managedAppRemediationAction 枚举类型
description: 要应用于托管应用程序的管理员启动的操作。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7c625ecde045860f49f06acff4513698fd82b474
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42781486"
---
# <a name="managedappremediationaction-enum-type"></a><span data-ttu-id="7c5a0-103">managedAppRemediationAction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="7c5a0-103">managedAppRemediationAction enum type</span></span>

> <span data-ttu-id="7c5a0-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7c5a0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c5a0-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7c5a0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c5a0-106">要应用于托管应用程序的管理员启动的操作。</span><span class="sxs-lookup"><span data-stu-id="7c5a0-106">An admin initiated action to be applied on a managed app.</span></span>

## <a name="members"></a><span data-ttu-id="7c5a0-107">成员</span><span class="sxs-lookup"><span data-stu-id="7c5a0-107">Members</span></span>
|<span data-ttu-id="7c5a0-108">成员</span><span class="sxs-lookup"><span data-stu-id="7c5a0-108">Member</span></span>|<span data-ttu-id="7c5a0-109">值</span><span class="sxs-lookup"><span data-stu-id="7c5a0-109">Value</span></span>|<span data-ttu-id="7c5a0-110">说明</span><span class="sxs-lookup"><span data-stu-id="7c5a0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c5a0-111">数据</span><span class="sxs-lookup"><span data-stu-id="7c5a0-111">block</span></span>|<span data-ttu-id="7c5a0-112">0</span><span class="sxs-lookup"><span data-stu-id="7c5a0-112">0</span></span>|<span data-ttu-id="7c5a0-113">要阻止的应用程序和相应的公司数据</span><span class="sxs-lookup"><span data-stu-id="7c5a0-113">app and the corresponding company data to be blocked</span></span>|
|<span data-ttu-id="7c5a0-114">擦</span><span class="sxs-lookup"><span data-stu-id="7c5a0-114">wipe</span></span>|<span data-ttu-id="7c5a0-115">1</span><span class="sxs-lookup"><span data-stu-id="7c5a0-115">1</span></span>|<span data-ttu-id="7c5a0-116">要擦除的应用程序和相应的公司数据</span><span class="sxs-lookup"><span data-stu-id="7c5a0-116">app and the corresponding company data to be wiped</span></span>|
|<span data-ttu-id="7c5a0-117">警告</span><span class="sxs-lookup"><span data-stu-id="7c5a0-117">warn</span></span>|<span data-ttu-id="7c5a0-118">双面</span><span class="sxs-lookup"><span data-stu-id="7c5a0-118">2</span></span>|<span data-ttu-id="7c5a0-119">要警告的应用程序和相应的用户</span><span class="sxs-lookup"><span data-stu-id="7c5a0-119">app and the corresponding user to be warned</span></span>|



