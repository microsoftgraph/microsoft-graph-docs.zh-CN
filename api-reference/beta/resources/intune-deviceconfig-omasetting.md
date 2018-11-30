---
title: omaSetting 资源类型
description: OMA 设置定义。
ms.openlocfilehash: 900e3f4d8e24743ed75b15f7a57188b46630c9fa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042733"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="66f2d-103">omaSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="66f2d-103">omaSetting resource type</span></span>

> <span data-ttu-id="66f2d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="66f2d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="66f2d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="66f2d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="66f2d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="66f2d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="66f2d-107">OMA 设置定义。</span><span class="sxs-lookup"><span data-stu-id="66f2d-107">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="66f2d-108">属性</span><span class="sxs-lookup"><span data-stu-id="66f2d-108">Properties</span></span>
|<span data-ttu-id="66f2d-109">属性</span><span class="sxs-lookup"><span data-stu-id="66f2d-109">Property</span></span>|<span data-ttu-id="66f2d-110">类型</span><span class="sxs-lookup"><span data-stu-id="66f2d-110">Type</span></span>|<span data-ttu-id="66f2d-111">说明</span><span class="sxs-lookup"><span data-stu-id="66f2d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66f2d-112">displayName</span><span class="sxs-lookup"><span data-stu-id="66f2d-112">displayName</span></span>|<span data-ttu-id="66f2d-113">String</span><span class="sxs-lookup"><span data-stu-id="66f2d-113">String</span></span>|<span data-ttu-id="66f2d-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="66f2d-114">Display Name.</span></span>|
|<span data-ttu-id="66f2d-115">description</span><span class="sxs-lookup"><span data-stu-id="66f2d-115">description</span></span>|<span data-ttu-id="66f2d-116">String</span><span class="sxs-lookup"><span data-stu-id="66f2d-116">String</span></span>|<span data-ttu-id="66f2d-117">说明。</span><span class="sxs-lookup"><span data-stu-id="66f2d-117">Description.</span></span>|
|<span data-ttu-id="66f2d-118">omaUri</span><span class="sxs-lookup"><span data-stu-id="66f2d-118">omaUri</span></span>|<span data-ttu-id="66f2d-119">String</span><span class="sxs-lookup"><span data-stu-id="66f2d-119">String</span></span>|<span data-ttu-id="66f2d-120">OMA。</span><span class="sxs-lookup"><span data-stu-id="66f2d-120">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66f2d-121">关系</span><span class="sxs-lookup"><span data-stu-id="66f2d-121">Relationships</span></span>
<span data-ttu-id="66f2d-122">无</span><span class="sxs-lookup"><span data-stu-id="66f2d-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="66f2d-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="66f2d-123">JSON Representation</span></span>
<span data-ttu-id="66f2d-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66f2d-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String"
}
```





