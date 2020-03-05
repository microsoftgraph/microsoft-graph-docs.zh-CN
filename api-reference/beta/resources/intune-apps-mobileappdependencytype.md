---
title: mobileAppDependencyType 枚举类型
description: 指示与两个移动应用程序之间的关系关联的依赖关系类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e008d01d4f53e5739412f279878d83cf7cc87d34
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42491702"
---
# <a name="mobileappdependencytype-enum-type"></a><span data-ttu-id="fd464-103">mobileAppDependencyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="fd464-103">mobileAppDependencyType enum type</span></span>

<span data-ttu-id="fd464-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="fd464-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fd464-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fd464-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fd464-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fd464-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd464-107">指示与两个移动应用程序之间的关系关联的依赖关系类型。</span><span class="sxs-lookup"><span data-stu-id="fd464-107">Indicates the dependency type associated with a relationship between two mobile apps.</span></span>

## <a name="members"></a><span data-ttu-id="fd464-108">成员</span><span class="sxs-lookup"><span data-stu-id="fd464-108">Members</span></span>
|<span data-ttu-id="fd464-109">成员</span><span class="sxs-lookup"><span data-stu-id="fd464-109">Member</span></span>|<span data-ttu-id="fd464-110">值</span><span class="sxs-lookup"><span data-stu-id="fd464-110">Value</span></span>|<span data-ttu-id="fd464-111">说明</span><span class="sxs-lookup"><span data-stu-id="fd464-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd464-112">出</span><span class="sxs-lookup"><span data-stu-id="fd464-112">detect</span></span>|<span data-ttu-id="fd464-113">0</span><span class="sxs-lookup"><span data-stu-id="fd464-113">0</span></span>|<span data-ttu-id="fd464-114">指示安装父应用程序之前应检测子应用程序。</span><span class="sxs-lookup"><span data-stu-id="fd464-114">Indicates that the child app should be detected before installing the parent app.</span></span>|
|<span data-ttu-id="fd464-115">安装</span><span class="sxs-lookup"><span data-stu-id="fd464-115">autoInstall</span></span>|<span data-ttu-id="fd464-116">1 </span><span class="sxs-lookup"><span data-stu-id="fd464-116">1</span></span>|<span data-ttu-id="fd464-117">指示安装父应用程序之前应安装子应用程序。</span><span class="sxs-lookup"><span data-stu-id="fd464-117">Indicates that the child app should be installed before installing the parent app.</span></span>|



