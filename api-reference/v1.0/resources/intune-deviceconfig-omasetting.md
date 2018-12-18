---
title: omaSetting 资源类型
description: OMA 设置定义。
author: tfitzmac
ms.openlocfilehash: 564912635fbcd5e2846965d3546a3830119db252
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340885"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="25928-103">omaSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="25928-103">omaSetting resource type</span></span>

> <span data-ttu-id="25928-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="25928-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="25928-105">OMA 设置定义。</span><span class="sxs-lookup"><span data-stu-id="25928-105">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="25928-106">属性</span><span class="sxs-lookup"><span data-stu-id="25928-106">Properties</span></span>
|<span data-ttu-id="25928-107">属性</span><span class="sxs-lookup"><span data-stu-id="25928-107">Property</span></span>|<span data-ttu-id="25928-108">类型</span><span class="sxs-lookup"><span data-stu-id="25928-108">Type</span></span>|<span data-ttu-id="25928-109">说明</span><span class="sxs-lookup"><span data-stu-id="25928-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25928-110">displayName</span><span class="sxs-lookup"><span data-stu-id="25928-110">displayName</span></span>|<span data-ttu-id="25928-111">String</span><span class="sxs-lookup"><span data-stu-id="25928-111">String</span></span>|<span data-ttu-id="25928-112">显示名称。</span><span class="sxs-lookup"><span data-stu-id="25928-112">Display Name.</span></span>|
|<span data-ttu-id="25928-113">description</span><span class="sxs-lookup"><span data-stu-id="25928-113">description</span></span>|<span data-ttu-id="25928-114">String</span><span class="sxs-lookup"><span data-stu-id="25928-114">String</span></span>|<span data-ttu-id="25928-115">说明。</span><span class="sxs-lookup"><span data-stu-id="25928-115">Description.</span></span>|
|<span data-ttu-id="25928-116">omaUri</span><span class="sxs-lookup"><span data-stu-id="25928-116">omaUri</span></span>|<span data-ttu-id="25928-117">String</span><span class="sxs-lookup"><span data-stu-id="25928-117">String</span></span>|<span data-ttu-id="25928-118">OMA。</span><span class="sxs-lookup"><span data-stu-id="25928-118">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="25928-119">关系</span><span class="sxs-lookup"><span data-stu-id="25928-119">Relationships</span></span>
<span data-ttu-id="25928-120">无</span><span class="sxs-lookup"><span data-stu-id="25928-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="25928-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="25928-121">JSON Representation</span></span>
<span data-ttu-id="25928-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="25928-122">Here is a JSON representation of the resource.</span></span>
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



