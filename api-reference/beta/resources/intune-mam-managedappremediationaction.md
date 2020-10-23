---
title: managedAppRemediationAction 枚举类型
description: 要应用于托管应用程序的管理员启动的操作。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 2e7b2e5f617d3c6dad194fb82273f6e0e47cb132
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48702381"
---
# <a name="managedappremediationaction-enum-type"></a><span data-ttu-id="332f6-103">managedAppRemediationAction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="332f6-103">managedAppRemediationAction enum type</span></span>

<span data-ttu-id="332f6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="332f6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="332f6-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="332f6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="332f6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="332f6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="332f6-107">要应用于托管应用程序的管理员启动的操作。</span><span class="sxs-lookup"><span data-stu-id="332f6-107">An admin initiated action to be applied on a managed app.</span></span>

## <a name="members"></a><span data-ttu-id="332f6-108">成员</span><span class="sxs-lookup"><span data-stu-id="332f6-108">Members</span></span>
|<span data-ttu-id="332f6-109">成员</span><span class="sxs-lookup"><span data-stu-id="332f6-109">Member</span></span>|<span data-ttu-id="332f6-110">值</span><span class="sxs-lookup"><span data-stu-id="332f6-110">Value</span></span>|<span data-ttu-id="332f6-111">说明</span><span class="sxs-lookup"><span data-stu-id="332f6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="332f6-112">数据</span><span class="sxs-lookup"><span data-stu-id="332f6-112">block</span></span>|<span data-ttu-id="332f6-113">0</span><span class="sxs-lookup"><span data-stu-id="332f6-113">0</span></span>|<span data-ttu-id="332f6-114">要阻止的应用程序和相应的公司数据</span><span class="sxs-lookup"><span data-stu-id="332f6-114">app and the corresponding company data to be blocked</span></span>|
|<span data-ttu-id="332f6-115">擦</span><span class="sxs-lookup"><span data-stu-id="332f6-115">wipe</span></span>|<span data-ttu-id="332f6-116">1</span><span class="sxs-lookup"><span data-stu-id="332f6-116">1</span></span>|<span data-ttu-id="332f6-117">要擦除的应用程序和相应的公司数据</span><span class="sxs-lookup"><span data-stu-id="332f6-117">app and the corresponding company data to be wiped</span></span>|
|<span data-ttu-id="332f6-118">警告</span><span class="sxs-lookup"><span data-stu-id="332f6-118">warn</span></span>|<span data-ttu-id="332f6-119">双面</span><span class="sxs-lookup"><span data-stu-id="332f6-119">2</span></span>|<span data-ttu-id="332f6-120">要警告的应用程序和相应的用户</span><span class="sxs-lookup"><span data-stu-id="332f6-120">app and the corresponding user to be warned</span></span>|





