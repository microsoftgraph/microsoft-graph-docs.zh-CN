---
title: keyValue 资源类型
description: 键值定义。
ms.openlocfilehash: 7279b48243139b9234b737ceb7d7fb1ad7232451
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043905"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="47e6f-103">keyValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="47e6f-103">keyValue resource type</span></span>

> <span data-ttu-id="47e6f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="47e6f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="47e6f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="47e6f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="47e6f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="47e6f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="47e6f-107">键值定义。</span><span class="sxs-lookup"><span data-stu-id="47e6f-107">Key Value definition.</span></span>
## <a name="properties"></a><span data-ttu-id="47e6f-108">属性</span><span class="sxs-lookup"><span data-stu-id="47e6f-108">Properties</span></span>
|<span data-ttu-id="47e6f-109">属性</span><span class="sxs-lookup"><span data-stu-id="47e6f-109">Property</span></span>|<span data-ttu-id="47e6f-110">类型</span><span class="sxs-lookup"><span data-stu-id="47e6f-110">Type</span></span>|<span data-ttu-id="47e6f-111">说明</span><span class="sxs-lookup"><span data-stu-id="47e6f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47e6f-112">Key</span><span class="sxs-lookup"><span data-stu-id="47e6f-112">key</span></span>|<span data-ttu-id="47e6f-113">字符串</span><span class="sxs-lookup"><span data-stu-id="47e6f-113">String</span></span>|<span data-ttu-id="47e6f-114">键。</span><span class="sxs-lookup"><span data-stu-id="47e6f-114">Key.</span></span>|
|<span data-ttu-id="47e6f-115">值</span><span class="sxs-lookup"><span data-stu-id="47e6f-115">value</span></span>|<span data-ttu-id="47e6f-116">String</span><span class="sxs-lookup"><span data-stu-id="47e6f-116">String</span></span>|<span data-ttu-id="47e6f-117">值。</span><span class="sxs-lookup"><span data-stu-id="47e6f-117">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="47e6f-118">关系</span><span class="sxs-lookup"><span data-stu-id="47e6f-118">Relationships</span></span>
<span data-ttu-id="47e6f-119">无</span><span class="sxs-lookup"><span data-stu-id="47e6f-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="47e6f-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="47e6f-120">JSON Representation</span></span>
<span data-ttu-id="47e6f-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="47e6f-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValue",
  "key": "String",
  "value": "String"
}
```





