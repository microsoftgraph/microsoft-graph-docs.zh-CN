---
title: managedAppRemediationAction 枚举类型
description: 管理员启动要应用于托管的应用程序的操作。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ecc4b61400cac841a9a699f2d8e3e99e2f543a74
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894199"
---
# <a name="managedappremediationaction-enum-type"></a><span data-ttu-id="0a7aa-103">managedAppRemediationAction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="0a7aa-103">managedAppRemediationAction enum type</span></span>

> <span data-ttu-id="0a7aa-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0a7aa-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a7aa-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0a7aa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0a7aa-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0a7aa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0a7aa-107">管理员启动要应用于托管的应用程序的操作。</span><span class="sxs-lookup"><span data-stu-id="0a7aa-107">An admin initiated action to be applied on a managed app.</span></span>
## <a name="members"></a><span data-ttu-id="0a7aa-108">成员</span><span class="sxs-lookup"><span data-stu-id="0a7aa-108">Members</span></span>
|<span data-ttu-id="0a7aa-109">成员</span><span class="sxs-lookup"><span data-stu-id="0a7aa-109">Member</span></span>|<span data-ttu-id="0a7aa-110">值</span><span class="sxs-lookup"><span data-stu-id="0a7aa-110">Value</span></span>|<span data-ttu-id="0a7aa-111">Description</span><span class="sxs-lookup"><span data-stu-id="0a7aa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a7aa-112">阻止</span><span class="sxs-lookup"><span data-stu-id="0a7aa-112">block</span></span>|<span data-ttu-id="0a7aa-113">0</span><span class="sxs-lookup"><span data-stu-id="0a7aa-113">0</span></span>|<span data-ttu-id="0a7aa-114">应用程序和相应的公司数据，可以被阻止</span><span class="sxs-lookup"><span data-stu-id="0a7aa-114">app and the corresponding company data to be blocked</span></span>|
|<span data-ttu-id="0a7aa-115">擦除</span><span class="sxs-lookup"><span data-stu-id="0a7aa-115">wipe</span></span>|<span data-ttu-id="0a7aa-116">1</span><span class="sxs-lookup"><span data-stu-id="0a7aa-116">1</span></span>|<span data-ttu-id="0a7aa-117">应用程序和相应的公司数据，要擦除</span><span class="sxs-lookup"><span data-stu-id="0a7aa-117">app and the corresponding company data to be wiped</span></span>|





