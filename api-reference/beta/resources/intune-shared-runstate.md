---
title: runState 枚举类型
description: 指示设备管理脚本执行状态的类型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4e83dbf367c1758c95ad02b0a0be8b5558e74f66
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425006"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="97bb9-103">runState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="97bb9-103">runState enum type</span></span>

> <span data-ttu-id="97bb9-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="97bb9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="97bb9-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="97bb9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="97bb9-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="97bb9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97bb9-107">指示设备管理脚本执行状态的类型。</span><span class="sxs-lookup"><span data-stu-id="97bb9-107">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="97bb9-108">成员</span><span class="sxs-lookup"><span data-stu-id="97bb9-108">Members</span></span>
|<span data-ttu-id="97bb9-109">成员</span><span class="sxs-lookup"><span data-stu-id="97bb9-109">Member</span></span>|<span data-ttu-id="97bb9-110">值</span><span class="sxs-lookup"><span data-stu-id="97bb9-110">Value</span></span>|<span data-ttu-id="97bb9-111">说明</span><span class="sxs-lookup"><span data-stu-id="97bb9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97bb9-112">unknown</span><span class="sxs-lookup"><span data-stu-id="97bb9-112">unknown</span></span>|<span data-ttu-id="97bb9-113">0</span><span class="sxs-lookup"><span data-stu-id="97bb9-113">0</span></span>|<span data-ttu-id="97bb9-114">未知的结果。</span><span class="sxs-lookup"><span data-stu-id="97bb9-114">Unknown result.</span></span>|
|<span data-ttu-id="97bb9-115">success</span><span class="sxs-lookup"><span data-stu-id="97bb9-115">success</span></span>|<span data-ttu-id="97bb9-116">1</span><span class="sxs-lookup"><span data-stu-id="97bb9-116">1</span></span>|<span data-ttu-id="97bb9-117">成功运行脚本。</span><span class="sxs-lookup"><span data-stu-id="97bb9-117">Script is run successfully.</span></span>|
|<span data-ttu-id="97bb9-118">失败</span><span class="sxs-lookup"><span data-stu-id="97bb9-118">fail</span></span>|<span data-ttu-id="97bb9-119">2</span><span class="sxs-lookup"><span data-stu-id="97bb9-119">2</span></span>|<span data-ttu-id="97bb9-120">运行脚本失败。</span><span class="sxs-lookup"><span data-stu-id="97bb9-120">Script failed to run.</span></span>|




