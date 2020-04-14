---
title: mobileAppDependencyType 枚举类型
description: 指示与两个移动应用程序之间的关系关联的依赖关系类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1a892b472d47765e9d570ad8096f771eee79e1a3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43440383"
---
# <a name="mobileappdependencytype-enum-type"></a><span data-ttu-id="8a988-103">mobileAppDependencyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="8a988-103">mobileAppDependencyType enum type</span></span>

<span data-ttu-id="8a988-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a988-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8a988-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8a988-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a988-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8a988-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a988-107">指示与两个移动应用程序之间的关系关联的依赖关系类型。</span><span class="sxs-lookup"><span data-stu-id="8a988-107">Indicates the dependency type associated with a relationship between two mobile apps.</span></span>

## <a name="members"></a><span data-ttu-id="8a988-108">成员</span><span class="sxs-lookup"><span data-stu-id="8a988-108">Members</span></span>
|<span data-ttu-id="8a988-109">成员</span><span class="sxs-lookup"><span data-stu-id="8a988-109">Member</span></span>|<span data-ttu-id="8a988-110">值</span><span class="sxs-lookup"><span data-stu-id="8a988-110">Value</span></span>|<span data-ttu-id="8a988-111">说明</span><span class="sxs-lookup"><span data-stu-id="8a988-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a988-112">出</span><span class="sxs-lookup"><span data-stu-id="8a988-112">detect</span></span>|<span data-ttu-id="8a988-113">0</span><span class="sxs-lookup"><span data-stu-id="8a988-113">0</span></span>|<span data-ttu-id="8a988-114">指示安装父应用程序之前应检测子应用程序。</span><span class="sxs-lookup"><span data-stu-id="8a988-114">Indicates that the child app should be detected before installing the parent app.</span></span>|
|<span data-ttu-id="8a988-115">安装</span><span class="sxs-lookup"><span data-stu-id="8a988-115">autoInstall</span></span>|<span data-ttu-id="8a988-116">1</span><span class="sxs-lookup"><span data-stu-id="8a988-116">1</span></span>|<span data-ttu-id="8a988-117">指示安装父应用程序之前应安装子应用程序。</span><span class="sxs-lookup"><span data-stu-id="8a988-117">Indicates that the child app should be installed before installing the parent app.</span></span>|



