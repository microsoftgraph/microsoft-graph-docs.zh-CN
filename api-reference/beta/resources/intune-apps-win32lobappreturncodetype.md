---
title: win32LobAppReturnCodeType 枚举类型
description: 指示返回代码的类型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 42491bd49759dbb7642fc968cd8957d5a2948305
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412385"
---
# <a name="win32lobappreturncodetype-enum-type"></a><span data-ttu-id="d141c-103">win32LobAppReturnCodeType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d141c-103">win32LobAppReturnCodeType enum type</span></span>

> <span data-ttu-id="d141c-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="d141c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d141c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d141c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d141c-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d141c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d141c-107">指示返回代码的类型。</span><span class="sxs-lookup"><span data-stu-id="d141c-107">Indicates the type of return code.</span></span>

## <a name="members"></a><span data-ttu-id="d141c-108">成员</span><span class="sxs-lookup"><span data-stu-id="d141c-108">Members</span></span>
|<span data-ttu-id="d141c-109">成员</span><span class="sxs-lookup"><span data-stu-id="d141c-109">Member</span></span>|<span data-ttu-id="d141c-110">值</span><span class="sxs-lookup"><span data-stu-id="d141c-110">Value</span></span>|<span data-ttu-id="d141c-111">说明</span><span class="sxs-lookup"><span data-stu-id="d141c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d141c-112">failed</span><span class="sxs-lookup"><span data-stu-id="d141c-112">failed</span></span>|<span data-ttu-id="d141c-113">0</span><span class="sxs-lookup"><span data-stu-id="d141c-113">0</span></span>|<span data-ttu-id="d141c-114">失败。</span><span class="sxs-lookup"><span data-stu-id="d141c-114">Failed.</span></span>|
|<span data-ttu-id="d141c-115">success</span><span class="sxs-lookup"><span data-stu-id="d141c-115">success</span></span>|<span data-ttu-id="d141c-116">1</span><span class="sxs-lookup"><span data-stu-id="d141c-116">1</span></span>|<span data-ttu-id="d141c-117">成功。</span><span class="sxs-lookup"><span data-stu-id="d141c-117">Success.</span></span>|
|<span data-ttu-id="d141c-118">softReboot</span><span class="sxs-lookup"><span data-stu-id="d141c-118">softReboot</span></span>|<span data-ttu-id="d141c-119">2</span><span class="sxs-lookup"><span data-stu-id="d141c-119">2</span></span>|<span data-ttu-id="d141c-120">软重启是必需的。</span><span class="sxs-lookup"><span data-stu-id="d141c-120">Soft-reboot is required.</span></span>|
|<span data-ttu-id="d141c-121">hardReboot</span><span class="sxs-lookup"><span data-stu-id="d141c-121">hardReboot</span></span>|<span data-ttu-id="d141c-122">3</span><span class="sxs-lookup"><span data-stu-id="d141c-122">3</span></span>|<span data-ttu-id="d141c-123">硬重新启动，则需要。</span><span class="sxs-lookup"><span data-stu-id="d141c-123">Hard-reboot is required.</span></span>|
|<span data-ttu-id="d141c-124">重试</span><span class="sxs-lookup"><span data-stu-id="d141c-124">retry</span></span>|<span data-ttu-id="d141c-125">4</span><span class="sxs-lookup"><span data-stu-id="d141c-125">4</span></span>|<span data-ttu-id="d141c-126">重试。</span><span class="sxs-lookup"><span data-stu-id="d141c-126">Retry.</span></span>|




