---
title: loggedOnUser 资源类型
description: 登录用户
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e8f1547669a2bb14c5ae84920c1eb6bef2dfbeb1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470519"
---
# <a name="loggedonuser-resource-type"></a><span data-ttu-id="d5793-103">loggedOnUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="d5793-103">loggedOnUser resource type</span></span>

<span data-ttu-id="d5793-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5793-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d5793-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d5793-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5793-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d5793-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5793-107">登录用户</span><span class="sxs-lookup"><span data-stu-id="d5793-107">Logged On User</span></span>

## <a name="properties"></a><span data-ttu-id="d5793-108">属性</span><span class="sxs-lookup"><span data-stu-id="d5793-108">Properties</span></span>
|<span data-ttu-id="d5793-109">属性</span><span class="sxs-lookup"><span data-stu-id="d5793-109">Property</span></span>|<span data-ttu-id="d5793-110">类型</span><span class="sxs-lookup"><span data-stu-id="d5793-110">Type</span></span>|<span data-ttu-id="d5793-111">说明</span><span class="sxs-lookup"><span data-stu-id="d5793-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5793-112">userId</span><span class="sxs-lookup"><span data-stu-id="d5793-112">userId</span></span>|<span data-ttu-id="d5793-113">String</span><span class="sxs-lookup"><span data-stu-id="d5793-113">String</span></span>|<span data-ttu-id="d5793-114">用户 ID</span><span class="sxs-lookup"><span data-stu-id="d5793-114">User id</span></span>|
|<span data-ttu-id="d5793-115">lastLogOnDateTime</span><span class="sxs-lookup"><span data-stu-id="d5793-115">lastLogOnDateTime</span></span>|<span data-ttu-id="d5793-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5793-116">DateTimeOffset</span></span>|<span data-ttu-id="d5793-117">用户登录的日期时间</span><span class="sxs-lookup"><span data-stu-id="d5793-117">Date time when user logs on</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5793-118">关系</span><span class="sxs-lookup"><span data-stu-id="d5793-118">Relationships</span></span>
<span data-ttu-id="d5793-119">无</span><span class="sxs-lookup"><span data-stu-id="d5793-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5793-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d5793-120">JSON Representation</span></span>
<span data-ttu-id="d5793-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d5793-121">Here is a JSON representation of the resource.</span></span>
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



