---
title: win32LobAppMsiPackageType 枚举类型
description: 指示 MSI Win32LobApp 的包类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e9c729c7a3d1e4d8a33136913f8c718b7e13b49d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42490614"
---
# <a name="win32lobappmsipackagetype-enum-type"></a><span data-ttu-id="dccbb-103">win32LobAppMsiPackageType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="dccbb-103">win32LobAppMsiPackageType enum type</span></span>

<span data-ttu-id="dccbb-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="dccbb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dccbb-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dccbb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dccbb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dccbb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dccbb-107">指示 MSI Win32LobApp 的包类型。</span><span class="sxs-lookup"><span data-stu-id="dccbb-107">Indicates the package type of an MSI Win32LobApp.</span></span>

## <a name="members"></a><span data-ttu-id="dccbb-108">成员</span><span class="sxs-lookup"><span data-stu-id="dccbb-108">Members</span></span>
|<span data-ttu-id="dccbb-109">成员</span><span class="sxs-lookup"><span data-stu-id="dccbb-109">Member</span></span>|<span data-ttu-id="dccbb-110">值</span><span class="sxs-lookup"><span data-stu-id="dccbb-110">Value</span></span>|<span data-ttu-id="dccbb-111">说明</span><span class="sxs-lookup"><span data-stu-id="dccbb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dccbb-112">perMachine</span><span class="sxs-lookup"><span data-stu-id="dccbb-112">perMachine</span></span>|<span data-ttu-id="dccbb-113">0</span><span class="sxs-lookup"><span data-stu-id="dccbb-113">0</span></span>|<span data-ttu-id="dccbb-114">指示每计算机应用程序包。</span><span class="sxs-lookup"><span data-stu-id="dccbb-114">Indicates a per-machine app package.</span></span>|
|<span data-ttu-id="dccbb-115">perUser</span><span class="sxs-lookup"><span data-stu-id="dccbb-115">perUser</span></span>|<span data-ttu-id="dccbb-116">1 </span><span class="sxs-lookup"><span data-stu-id="dccbb-116">1</span></span>|<span data-ttu-id="dccbb-117">指示每用户应用程序包。</span><span class="sxs-lookup"><span data-stu-id="dccbb-117">Indicates a per-user app package.</span></span>|
|<span data-ttu-id="dccbb-118">dualPurpose</span><span class="sxs-lookup"><span data-stu-id="dccbb-118">dualPurpose</span></span>|<span data-ttu-id="dccbb-119">2 </span><span class="sxs-lookup"><span data-stu-id="dccbb-119">2</span></span>|<span data-ttu-id="dccbb-120">指示一个双用途应用程序包。</span><span class="sxs-lookup"><span data-stu-id="dccbb-120">Indicates a dual-purpose app package.</span></span>|



