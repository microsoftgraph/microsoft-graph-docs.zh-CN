---
title: mobileAppDependecyType 枚举类型
description: 指示与两个移动应用程序之间的关系关联的依赖关系类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0cbf468435aa289913b566750823e65c73249838
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554175"
---
# <a name="mobileappdependecytype-enum-type"></a><span data-ttu-id="e3b0f-103">mobileAppDependecyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e3b0f-103">mobileAppDependecyType enum type</span></span>

> <span data-ttu-id="e3b0f-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e3b0f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3b0f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e3b0f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3b0f-106">指示与两个移动应用程序之间的关系关联的依赖关系类型。</span><span class="sxs-lookup"><span data-stu-id="e3b0f-106">Indicates the dependency type associated with a relationship between two mobile apps.</span></span>

## <a name="members"></a><span data-ttu-id="e3b0f-107">成员</span><span class="sxs-lookup"><span data-stu-id="e3b0f-107">Members</span></span>
|<span data-ttu-id="e3b0f-108">成员</span><span class="sxs-lookup"><span data-stu-id="e3b0f-108">Member</span></span>|<span data-ttu-id="e3b0f-109">值</span><span class="sxs-lookup"><span data-stu-id="e3b0f-109">Value</span></span>|<span data-ttu-id="e3b0f-110">说明</span><span class="sxs-lookup"><span data-stu-id="e3b0f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3b0f-111">出</span><span class="sxs-lookup"><span data-stu-id="e3b0f-111">detect</span></span>|<span data-ttu-id="e3b0f-112">0</span><span class="sxs-lookup"><span data-stu-id="e3b0f-112">0</span></span>|<span data-ttu-id="e3b0f-113">指示安装父应用程序之前应检测子应用程序。</span><span class="sxs-lookup"><span data-stu-id="e3b0f-113">Indicates that the child app should be detected before installing the parent app.</span></span>|
|<span data-ttu-id="e3b0f-114">安装</span><span class="sxs-lookup"><span data-stu-id="e3b0f-114">autoInstall</span></span>|<span data-ttu-id="e3b0f-115">1</span><span class="sxs-lookup"><span data-stu-id="e3b0f-115">1</span></span>|<span data-ttu-id="e3b0f-116">指示安装父应用程序之前应安装子应用程序。</span><span class="sxs-lookup"><span data-stu-id="e3b0f-116">Indicates that the child app should be installed before installing the parent app.</span></span>|





