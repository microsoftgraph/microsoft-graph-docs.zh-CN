---
title: mobileAppSupersedenceType 枚举类型
description: 指示与两个移动应用程序之间的关系关联的取代类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: aa947a2d5ad5b580de49180fee573a4f7d395952
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733285"
---
# <a name="mobileappsupersedencetype-enum-type"></a><span data-ttu-id="8ea06-103">mobileAppSupersedenceType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="8ea06-103">mobileAppSupersedenceType enum type</span></span>

<span data-ttu-id="8ea06-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ea06-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ea06-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8ea06-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ea06-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8ea06-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ea06-107">指示与两个移动应用程序之间的关系关联的取代类型。</span><span class="sxs-lookup"><span data-stu-id="8ea06-107">Indicates the supersedence type associated with a relationship between two mobile apps.</span></span>

## <a name="members"></a><span data-ttu-id="8ea06-108">成员</span><span class="sxs-lookup"><span data-stu-id="8ea06-108">Members</span></span>
|<span data-ttu-id="8ea06-109">成员</span><span class="sxs-lookup"><span data-stu-id="8ea06-109">Member</span></span>|<span data-ttu-id="8ea06-110">值</span><span class="sxs-lookup"><span data-stu-id="8ea06-110">Value</span></span>|<span data-ttu-id="8ea06-111">说明</span><span class="sxs-lookup"><span data-stu-id="8ea06-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ea06-112">最新更新</span><span class="sxs-lookup"><span data-stu-id="8ea06-112">update</span></span>|<span data-ttu-id="8ea06-113">0</span><span class="sxs-lookup"><span data-stu-id="8ea06-113">0</span></span>|<span data-ttu-id="8ea06-114">指示子应用程序应由父应用程序的内部逻辑进行更新。</span><span class="sxs-lookup"><span data-stu-id="8ea06-114">Indicates that the child app should be updated by the internal logic of the parent app.</span></span>|
|<span data-ttu-id="8ea06-115">replace</span><span class="sxs-lookup"><span data-stu-id="8ea06-115">replace</span></span>|<span data-ttu-id="8ea06-116">1</span><span class="sxs-lookup"><span data-stu-id="8ea06-116">1</span></span>|<span data-ttu-id="8ea06-117">指示安装父应用程序之前应卸载子应用程序。</span><span class="sxs-lookup"><span data-stu-id="8ea06-117">Indicates that the child app should be uninstalled before installing the parent app.</span></span>|





