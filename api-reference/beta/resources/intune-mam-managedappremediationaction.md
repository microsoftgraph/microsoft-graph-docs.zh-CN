---
title: managedAppRemediationAction 枚举类型
description: 要应用于托管应用程序的管理员启动的操作。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f6def057a694971d74089b5a9bde821d9d98ae0f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43371967"
---
# <a name="managedappremediationaction-enum-type"></a><span data-ttu-id="bd8f1-103">managedAppRemediationAction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="bd8f1-103">managedAppRemediationAction enum type</span></span>

<span data-ttu-id="bd8f1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd8f1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bd8f1-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bd8f1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd8f1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bd8f1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd8f1-107">要应用于托管应用程序的管理员启动的操作。</span><span class="sxs-lookup"><span data-stu-id="bd8f1-107">An admin initiated action to be applied on a managed app.</span></span>

## <a name="members"></a><span data-ttu-id="bd8f1-108">成员</span><span class="sxs-lookup"><span data-stu-id="bd8f1-108">Members</span></span>
|<span data-ttu-id="bd8f1-109">成员</span><span class="sxs-lookup"><span data-stu-id="bd8f1-109">Member</span></span>|<span data-ttu-id="bd8f1-110">值</span><span class="sxs-lookup"><span data-stu-id="bd8f1-110">Value</span></span>|<span data-ttu-id="bd8f1-111">说明</span><span class="sxs-lookup"><span data-stu-id="bd8f1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd8f1-112">数据</span><span class="sxs-lookup"><span data-stu-id="bd8f1-112">block</span></span>|<span data-ttu-id="bd8f1-113">0</span><span class="sxs-lookup"><span data-stu-id="bd8f1-113">0</span></span>|<span data-ttu-id="bd8f1-114">要阻止的应用程序和相应的公司数据</span><span class="sxs-lookup"><span data-stu-id="bd8f1-114">app and the corresponding company data to be blocked</span></span>|
|<span data-ttu-id="bd8f1-115">擦</span><span class="sxs-lookup"><span data-stu-id="bd8f1-115">wipe</span></span>|<span data-ttu-id="bd8f1-116">1</span><span class="sxs-lookup"><span data-stu-id="bd8f1-116">1</span></span>|<span data-ttu-id="bd8f1-117">要擦除的应用程序和相应的公司数据</span><span class="sxs-lookup"><span data-stu-id="bd8f1-117">app and the corresponding company data to be wiped</span></span>|
|<span data-ttu-id="bd8f1-118">警告</span><span class="sxs-lookup"><span data-stu-id="bd8f1-118">warn</span></span>|<span data-ttu-id="bd8f1-119">双面</span><span class="sxs-lookup"><span data-stu-id="bd8f1-119">2</span></span>|<span data-ttu-id="bd8f1-120">要警告的应用程序和相应的用户</span><span class="sxs-lookup"><span data-stu-id="bd8f1-120">app and the corresponding user to be warned</span></span>|



