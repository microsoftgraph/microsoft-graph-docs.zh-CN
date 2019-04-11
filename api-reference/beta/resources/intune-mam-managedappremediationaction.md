---
title: managedAppRemediationAction 枚举类型
description: 要应用于托管应用程序的管理员启动的操作。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1eb9643fc1b4c8c4ec858fd00b0a65a40c225307
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31791262"
---
# <a name="managedappremediationaction-enum-type"></a><span data-ttu-id="3e571-103">managedAppRemediationAction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3e571-103">managedAppRemediationAction enum type</span></span>

> <span data-ttu-id="3e571-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3e571-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e571-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3e571-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e571-106">要应用于托管应用程序的管理员启动的操作。</span><span class="sxs-lookup"><span data-stu-id="3e571-106">An admin initiated action to be applied on a managed app.</span></span>

## <a name="members"></a><span data-ttu-id="3e571-107">成员</span><span class="sxs-lookup"><span data-stu-id="3e571-107">Members</span></span>
|<span data-ttu-id="3e571-108">成员</span><span class="sxs-lookup"><span data-stu-id="3e571-108">Member</span></span>|<span data-ttu-id="3e571-109">值</span><span class="sxs-lookup"><span data-stu-id="3e571-109">Value</span></span>|<span data-ttu-id="3e571-110">说明</span><span class="sxs-lookup"><span data-stu-id="3e571-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e571-111">数据</span><span class="sxs-lookup"><span data-stu-id="3e571-111">block</span></span>|<span data-ttu-id="3e571-112">0</span><span class="sxs-lookup"><span data-stu-id="3e571-112">0</span></span>|<span data-ttu-id="3e571-113">要阻止的应用程序和相应的公司数据</span><span class="sxs-lookup"><span data-stu-id="3e571-113">app and the corresponding company data to be blocked</span></span>|
|<span data-ttu-id="3e571-114">擦</span><span class="sxs-lookup"><span data-stu-id="3e571-114">wipe</span></span>|<span data-ttu-id="3e571-115">1</span><span class="sxs-lookup"><span data-stu-id="3e571-115">1</span></span>|<span data-ttu-id="3e571-116">要擦除的应用程序和相应的公司数据</span><span class="sxs-lookup"><span data-stu-id="3e571-116">app and the corresponding company data to be wiped</span></span>|
|<span data-ttu-id="3e571-117">警告</span><span class="sxs-lookup"><span data-stu-id="3e571-117">warn</span></span>|<span data-ttu-id="3e571-118">双面</span><span class="sxs-lookup"><span data-stu-id="3e571-118">2</span></span>|<span data-ttu-id="3e571-119">要警告的应用程序和相应的用户</span><span class="sxs-lookup"><span data-stu-id="3e571-119">app and the corresponding user to be warned</span></span>|





