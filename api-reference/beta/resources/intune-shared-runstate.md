---
title: runState 枚举类型
description: 指示设备管理脚本的执行状态的类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d77f3ef9a2d7fd37edeaf2b4cc25d5e6d5bfcf4f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347848"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="20661-103">runState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="20661-103">runState enum type</span></span>

> <span data-ttu-id="20661-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="20661-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20661-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="20661-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20661-106">指示设备管理脚本的执行状态的类型。</span><span class="sxs-lookup"><span data-stu-id="20661-106">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="20661-107">成员</span><span class="sxs-lookup"><span data-stu-id="20661-107">Members</span></span>
|<span data-ttu-id="20661-108">成员</span><span class="sxs-lookup"><span data-stu-id="20661-108">Member</span></span>|<span data-ttu-id="20661-109">值</span><span class="sxs-lookup"><span data-stu-id="20661-109">Value</span></span>|<span data-ttu-id="20661-110">说明</span><span class="sxs-lookup"><span data-stu-id="20661-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20661-111">unknown</span><span class="sxs-lookup"><span data-stu-id="20661-111">unknown</span></span>|<span data-ttu-id="20661-112">0</span><span class="sxs-lookup"><span data-stu-id="20661-112">0</span></span>|<span data-ttu-id="20661-113">未知结果。</span><span class="sxs-lookup"><span data-stu-id="20661-113">Unknown result.</span></span>|
|<span data-ttu-id="20661-114">success</span><span class="sxs-lookup"><span data-stu-id="20661-114">success</span></span>|<span data-ttu-id="20661-115">1</span><span class="sxs-lookup"><span data-stu-id="20661-115">1</span></span>|<span data-ttu-id="20661-116">脚本成功运行。</span><span class="sxs-lookup"><span data-stu-id="20661-116">Script is run successfully.</span></span>|
|<span data-ttu-id="20661-117">失败</span><span class="sxs-lookup"><span data-stu-id="20661-117">fail</span></span>|<span data-ttu-id="20661-118">双面</span><span class="sxs-lookup"><span data-stu-id="20661-118">2</span></span>|<span data-ttu-id="20661-119">脚本运行失败。</span><span class="sxs-lookup"><span data-stu-id="20661-119">Script failed to run.</span></span>|
|<span data-ttu-id="20661-120">error</span><span class="sxs-lookup"><span data-stu-id="20661-120">error</span></span>|<span data-ttu-id="20661-121">第三章</span><span class="sxs-lookup"><span data-stu-id="20661-121">3</span></span>|<span data-ttu-id="20661-122">发现脚本命中错误。</span><span class="sxs-lookup"><span data-stu-id="20661-122">Discovery script hits error.</span></span>|
|<span data-ttu-id="20661-123">决</span><span class="sxs-lookup"><span data-stu-id="20661-123">pending</span></span>|<span data-ttu-id="20661-124">4</span><span class="sxs-lookup"><span data-stu-id="20661-124">4</span></span>|<span data-ttu-id="20661-125">脚本正在挂起中执行。</span><span class="sxs-lookup"><span data-stu-id="20661-125">Script is pending to execute.</span></span>|



