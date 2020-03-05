---
title: managedAppRemediationAction 枚举类型
description: 要应用于托管应用程序的管理员启动的操作。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 92fb38fa7b165359e3ed5e378da4e14b2f26095f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527880"
---
# <a name="managedappremediationaction-enum-type"></a><span data-ttu-id="ee4ea-103">managedAppRemediationAction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ee4ea-103">managedAppRemediationAction enum type</span></span>

<span data-ttu-id="ee4ea-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ee4ea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ee4ea-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ee4ea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee4ea-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ee4ea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee4ea-107">要应用于托管应用程序的管理员启动的操作。</span><span class="sxs-lookup"><span data-stu-id="ee4ea-107">An admin initiated action to be applied on a managed app.</span></span>

## <a name="members"></a><span data-ttu-id="ee4ea-108">成员</span><span class="sxs-lookup"><span data-stu-id="ee4ea-108">Members</span></span>
|<span data-ttu-id="ee4ea-109">成员</span><span class="sxs-lookup"><span data-stu-id="ee4ea-109">Member</span></span>|<span data-ttu-id="ee4ea-110">值</span><span class="sxs-lookup"><span data-stu-id="ee4ea-110">Value</span></span>|<span data-ttu-id="ee4ea-111">说明</span><span class="sxs-lookup"><span data-stu-id="ee4ea-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee4ea-112">数据</span><span class="sxs-lookup"><span data-stu-id="ee4ea-112">block</span></span>|<span data-ttu-id="ee4ea-113">0</span><span class="sxs-lookup"><span data-stu-id="ee4ea-113">0</span></span>|<span data-ttu-id="ee4ea-114">要阻止的应用程序和相应的公司数据</span><span class="sxs-lookup"><span data-stu-id="ee4ea-114">app and the corresponding company data to be blocked</span></span>|
|<span data-ttu-id="ee4ea-115">擦</span><span class="sxs-lookup"><span data-stu-id="ee4ea-115">wipe</span></span>|<span data-ttu-id="ee4ea-116">1 </span><span class="sxs-lookup"><span data-stu-id="ee4ea-116">1</span></span>|<span data-ttu-id="ee4ea-117">要擦除的应用程序和相应的公司数据</span><span class="sxs-lookup"><span data-stu-id="ee4ea-117">app and the corresponding company data to be wiped</span></span>|
|<span data-ttu-id="ee4ea-118">警告</span><span class="sxs-lookup"><span data-stu-id="ee4ea-118">warn</span></span>|<span data-ttu-id="ee4ea-119">2 </span><span class="sxs-lookup"><span data-stu-id="ee4ea-119">2</span></span>|<span data-ttu-id="ee4ea-120">要警告的应用程序和相应的用户</span><span class="sxs-lookup"><span data-stu-id="ee4ea-120">app and the corresponding user to be warned</span></span>|



