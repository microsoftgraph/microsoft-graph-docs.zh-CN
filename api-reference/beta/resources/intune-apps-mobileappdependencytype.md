---
title: mobileAppDependencyType 枚举类型
description: 指示与两个移动应用程序之间的关系关联的依赖关系类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 65a9c30b1aadbd7003e39e098d4e850675bea718
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34957638"
---
# <a name="mobileappdependencytype-enum-type"></a><span data-ttu-id="5f5ba-103">mobileAppDependencyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5f5ba-103">mobileAppDependencyType enum type</span></span>

> <span data-ttu-id="5f5ba-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5f5ba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f5ba-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5f5ba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f5ba-106">指示与两个移动应用程序之间的关系关联的依赖关系类型。</span><span class="sxs-lookup"><span data-stu-id="5f5ba-106">Indicates the dependency type associated with a relationship between two mobile apps.</span></span>

## <a name="members"></a><span data-ttu-id="5f5ba-107">成员</span><span class="sxs-lookup"><span data-stu-id="5f5ba-107">Members</span></span>
|<span data-ttu-id="5f5ba-108">成员</span><span class="sxs-lookup"><span data-stu-id="5f5ba-108">Member</span></span>|<span data-ttu-id="5f5ba-109">值</span><span class="sxs-lookup"><span data-stu-id="5f5ba-109">Value</span></span>|<span data-ttu-id="5f5ba-110">说明</span><span class="sxs-lookup"><span data-stu-id="5f5ba-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f5ba-111">出</span><span class="sxs-lookup"><span data-stu-id="5f5ba-111">detect</span></span>|<span data-ttu-id="5f5ba-112">0</span><span class="sxs-lookup"><span data-stu-id="5f5ba-112">0</span></span>|<span data-ttu-id="5f5ba-113">指示安装父应用程序之前应检测子应用程序。</span><span class="sxs-lookup"><span data-stu-id="5f5ba-113">Indicates that the child app should be detected before installing the parent app.</span></span>|
|<span data-ttu-id="5f5ba-114">安装</span><span class="sxs-lookup"><span data-stu-id="5f5ba-114">autoInstall</span></span>|<span data-ttu-id="5f5ba-115">1</span><span class="sxs-lookup"><span data-stu-id="5f5ba-115">1</span></span>|<span data-ttu-id="5f5ba-116">指示安装父应用程序之前应安装子应用程序。</span><span class="sxs-lookup"><span data-stu-id="5f5ba-116">Indicates that the child app should be installed before installing the parent app.</span></span>|





