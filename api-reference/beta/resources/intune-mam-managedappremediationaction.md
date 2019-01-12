---
title: managedAppRemediationAction 枚举类型
description: 管理员启动要应用于托管的应用程序的操作。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1abfe8e05eaa93d7588ae38e2fd5944a106fca32
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967152"
---
# <a name="managedappremediationaction-enum-type"></a><span data-ttu-id="7ce8c-103">managedAppRemediationAction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="7ce8c-103">managedAppRemediationAction enum type</span></span>

> <span data-ttu-id="7ce8c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7ce8c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ce8c-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7ce8c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7ce8c-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7ce8c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7ce8c-107">管理员启动要应用于托管的应用程序的操作。</span><span class="sxs-lookup"><span data-stu-id="7ce8c-107">An admin initiated action to be applied on a managed app.</span></span>
## <a name="members"></a><span data-ttu-id="7ce8c-108">成员</span><span class="sxs-lookup"><span data-stu-id="7ce8c-108">Members</span></span>
|<span data-ttu-id="7ce8c-109">成员</span><span class="sxs-lookup"><span data-stu-id="7ce8c-109">Member</span></span>|<span data-ttu-id="7ce8c-110">值</span><span class="sxs-lookup"><span data-stu-id="7ce8c-110">Value</span></span>|<span data-ttu-id="7ce8c-111">Description</span><span class="sxs-lookup"><span data-stu-id="7ce8c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ce8c-112">阻止</span><span class="sxs-lookup"><span data-stu-id="7ce8c-112">block</span></span>|<span data-ttu-id="7ce8c-113">0</span><span class="sxs-lookup"><span data-stu-id="7ce8c-113">0</span></span>|<span data-ttu-id="7ce8c-114">应用程序和相应的公司数据，可以被阻止</span><span class="sxs-lookup"><span data-stu-id="7ce8c-114">app and the corresponding company data to be blocked</span></span>|
|<span data-ttu-id="7ce8c-115">擦除</span><span class="sxs-lookup"><span data-stu-id="7ce8c-115">wipe</span></span>|<span data-ttu-id="7ce8c-116">1</span><span class="sxs-lookup"><span data-stu-id="7ce8c-116">1</span></span>|<span data-ttu-id="7ce8c-117">应用程序和相应的公司数据，要擦除</span><span class="sxs-lookup"><span data-stu-id="7ce8c-117">app and the corresponding company data to be wiped</span></span>|





