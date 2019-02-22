---
title: loggedOnUser 资源类型
description: 登录用户
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a5dfaa8bbaa879fc48c5f6ea31d1b7b14e998820
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148928"
---
# <a name="loggedonuser-resource-type"></a><span data-ttu-id="6d7a1-103">loggedOnUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="6d7a1-103">loggedOnUser resource type</span></span>

> <span data-ttu-id="6d7a1-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6d7a1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d7a1-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6d7a1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d7a1-106">登录用户</span><span class="sxs-lookup"><span data-stu-id="6d7a1-106">Logged On User</span></span>

## <a name="properties"></a><span data-ttu-id="6d7a1-107">属性</span><span class="sxs-lookup"><span data-stu-id="6d7a1-107">Properties</span></span>
|<span data-ttu-id="6d7a1-108">属性</span><span class="sxs-lookup"><span data-stu-id="6d7a1-108">Property</span></span>|<span data-ttu-id="6d7a1-109">类型</span><span class="sxs-lookup"><span data-stu-id="6d7a1-109">Type</span></span>|<span data-ttu-id="6d7a1-110">说明</span><span class="sxs-lookup"><span data-stu-id="6d7a1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d7a1-111">userId</span><span class="sxs-lookup"><span data-stu-id="6d7a1-111">userId</span></span>|<span data-ttu-id="6d7a1-112">String</span><span class="sxs-lookup"><span data-stu-id="6d7a1-112">String</span></span>|<span data-ttu-id="6d7a1-113">用户 id</span><span class="sxs-lookup"><span data-stu-id="6d7a1-113">User id</span></span>|
|<span data-ttu-id="6d7a1-114">lastLogOnDateTime</span><span class="sxs-lookup"><span data-stu-id="6d7a1-114">lastLogOnDateTime</span></span>|<span data-ttu-id="6d7a1-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d7a1-115">DateTimeOffset</span></span>|<span data-ttu-id="6d7a1-116">用户登录的日期时间</span><span class="sxs-lookup"><span data-stu-id="6d7a1-116">Date time when user logs on</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d7a1-117">关系</span><span class="sxs-lookup"><span data-stu-id="6d7a1-117">Relationships</span></span>
<span data-ttu-id="6d7a1-118">无</span><span class="sxs-lookup"><span data-stu-id="6d7a1-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6d7a1-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6d7a1-119">JSON Representation</span></span>
<span data-ttu-id="6d7a1-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d7a1-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.loggedOnUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.loggedOnUser",
  "userId": "String",
  "lastLogOnDateTime": "String (timestamp)"
}
```




