---
title: win32LobAppMsiPackageType 枚举类型
description: 指示 MSI Win32LobApp 的包类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3902604561fef4d26f3103d5ffe8c66701ef56a0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43422941"
---
# <a name="win32lobappmsipackagetype-enum-type"></a><span data-ttu-id="75f31-103">win32LobAppMsiPackageType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="75f31-103">win32LobAppMsiPackageType enum type</span></span>

<span data-ttu-id="75f31-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75f31-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75f31-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="75f31-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75f31-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="75f31-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75f31-107">指示 MSI Win32LobApp 的包类型。</span><span class="sxs-lookup"><span data-stu-id="75f31-107">Indicates the package type of an MSI Win32LobApp.</span></span>

## <a name="members"></a><span data-ttu-id="75f31-108">成员</span><span class="sxs-lookup"><span data-stu-id="75f31-108">Members</span></span>
|<span data-ttu-id="75f31-109">成员</span><span class="sxs-lookup"><span data-stu-id="75f31-109">Member</span></span>|<span data-ttu-id="75f31-110">值</span><span class="sxs-lookup"><span data-stu-id="75f31-110">Value</span></span>|<span data-ttu-id="75f31-111">说明</span><span class="sxs-lookup"><span data-stu-id="75f31-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75f31-112">perMachine</span><span class="sxs-lookup"><span data-stu-id="75f31-112">perMachine</span></span>|<span data-ttu-id="75f31-113">0</span><span class="sxs-lookup"><span data-stu-id="75f31-113">0</span></span>|<span data-ttu-id="75f31-114">指示每计算机应用程序包。</span><span class="sxs-lookup"><span data-stu-id="75f31-114">Indicates a per-machine app package.</span></span>|
|<span data-ttu-id="75f31-115">perUser</span><span class="sxs-lookup"><span data-stu-id="75f31-115">perUser</span></span>|<span data-ttu-id="75f31-116">1</span><span class="sxs-lookup"><span data-stu-id="75f31-116">1</span></span>|<span data-ttu-id="75f31-117">指示每用户应用程序包。</span><span class="sxs-lookup"><span data-stu-id="75f31-117">Indicates a per-user app package.</span></span>|
|<span data-ttu-id="75f31-118">dualPurpose</span><span class="sxs-lookup"><span data-stu-id="75f31-118">dualPurpose</span></span>|<span data-ttu-id="75f31-119">双面</span><span class="sxs-lookup"><span data-stu-id="75f31-119">2</span></span>|<span data-ttu-id="75f31-120">指示一个双用途应用程序包。</span><span class="sxs-lookup"><span data-stu-id="75f31-120">Indicates a dual-purpose app package.</span></span>|



