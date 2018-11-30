---
title: resourceAction 资源类型
description: 尚未记录
ms.openlocfilehash: 4cbfc149207f2f7589bd7e05075326641d4e8b67
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007715"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="67511-103">resourceAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="67511-103">resourceAction resource type</span></span>

> <span data-ttu-id="67511-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="67511-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="67511-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="67511-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="67511-106">属性</span><span class="sxs-lookup"><span data-stu-id="67511-106">Properties</span></span>
|<span data-ttu-id="67511-107">属性</span><span class="sxs-lookup"><span data-stu-id="67511-107">Property</span></span>|<span data-ttu-id="67511-108">类型</span><span class="sxs-lookup"><span data-stu-id="67511-108">Type</span></span>|<span data-ttu-id="67511-109">说明</span><span class="sxs-lookup"><span data-stu-id="67511-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67511-110">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="67511-110">allowedResourceActions</span></span>|<span data-ttu-id="67511-111">字符串集合</span><span class="sxs-lookup"><span data-stu-id="67511-111">String collection</span></span>|<span data-ttu-id="67511-112">允许的操作</span><span class="sxs-lookup"><span data-stu-id="67511-112">Allowed Actions</span></span>|
|<span data-ttu-id="67511-113">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="67511-113">notAllowedResourceActions</span></span>|<span data-ttu-id="67511-114">字符串集合</span><span class="sxs-lookup"><span data-stu-id="67511-114">String collection</span></span>|<span data-ttu-id="67511-115">不允许的操作</span><span class="sxs-lookup"><span data-stu-id="67511-115">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="67511-116">关系</span><span class="sxs-lookup"><span data-stu-id="67511-116">Relationships</span></span>
<span data-ttu-id="67511-117">无</span><span class="sxs-lookup"><span data-stu-id="67511-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="67511-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="67511-118">JSON Representation</span></span>
<span data-ttu-id="67511-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="67511-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```



