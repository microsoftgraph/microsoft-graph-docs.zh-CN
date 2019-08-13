---
title: loggedOnUser 资源类型
description: 登录用户
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a32ee6182f8937123662e3a8c3e4d18145607151
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372326"
---
# <a name="loggedonuser-resource-type"></a><span data-ttu-id="f58d7-103">loggedOnUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="f58d7-103">loggedOnUser resource type</span></span>

> <span data-ttu-id="f58d7-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f58d7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f58d7-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f58d7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f58d7-106">登录用户</span><span class="sxs-lookup"><span data-stu-id="f58d7-106">Logged On User</span></span>

## <a name="properties"></a><span data-ttu-id="f58d7-107">属性</span><span class="sxs-lookup"><span data-stu-id="f58d7-107">Properties</span></span>
|<span data-ttu-id="f58d7-108">属性</span><span class="sxs-lookup"><span data-stu-id="f58d7-108">Property</span></span>|<span data-ttu-id="f58d7-109">类型</span><span class="sxs-lookup"><span data-stu-id="f58d7-109">Type</span></span>|<span data-ttu-id="f58d7-110">说明</span><span class="sxs-lookup"><span data-stu-id="f58d7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f58d7-111">userId</span><span class="sxs-lookup"><span data-stu-id="f58d7-111">userId</span></span>|<span data-ttu-id="f58d7-112">String</span><span class="sxs-lookup"><span data-stu-id="f58d7-112">String</span></span>|<span data-ttu-id="f58d7-113">用户 ID</span><span class="sxs-lookup"><span data-stu-id="f58d7-113">User id</span></span>|
|<span data-ttu-id="f58d7-114">lastLogOnDateTime</span><span class="sxs-lookup"><span data-stu-id="f58d7-114">lastLogOnDateTime</span></span>|<span data-ttu-id="f58d7-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f58d7-115">DateTimeOffset</span></span>|<span data-ttu-id="f58d7-116">用户登录的日期时间</span><span class="sxs-lookup"><span data-stu-id="f58d7-116">Date time when user logs on</span></span>|

## <a name="relationships"></a><span data-ttu-id="f58d7-117">关系</span><span class="sxs-lookup"><span data-stu-id="f58d7-117">Relationships</span></span>
<span data-ttu-id="f58d7-118">无</span><span class="sxs-lookup"><span data-stu-id="f58d7-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f58d7-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f58d7-119">JSON Representation</span></span>
<span data-ttu-id="f58d7-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f58d7-120">Here is a JSON representation of the resource.</span></span>
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



