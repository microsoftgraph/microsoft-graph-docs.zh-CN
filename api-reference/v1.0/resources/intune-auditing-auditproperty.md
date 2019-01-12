---
title: auditProperty 资源类型
description: 包含审核属性的属性的类。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 290aae8c245fd09c17fc766cedd7c2e253626943
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912027"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="02231-103">auditProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="02231-103">auditProperty resource type</span></span>

> <span data-ttu-id="02231-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="02231-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="02231-105">包含审核属性的属性的类。</span><span class="sxs-lookup"><span data-stu-id="02231-105">A class containing the properties for Audit Property.</span></span>
## <a name="properties"></a><span data-ttu-id="02231-106">属性</span><span class="sxs-lookup"><span data-stu-id="02231-106">Properties</span></span>
|<span data-ttu-id="02231-107">属性</span><span class="sxs-lookup"><span data-stu-id="02231-107">Property</span></span>|<span data-ttu-id="02231-108">类型</span><span class="sxs-lookup"><span data-stu-id="02231-108">Type</span></span>|<span data-ttu-id="02231-109">说明</span><span class="sxs-lookup"><span data-stu-id="02231-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02231-110">displayName</span><span class="sxs-lookup"><span data-stu-id="02231-110">displayName</span></span>|<span data-ttu-id="02231-111">String</span><span class="sxs-lookup"><span data-stu-id="02231-111">String</span></span>|<span data-ttu-id="02231-112">显示名称。</span><span class="sxs-lookup"><span data-stu-id="02231-112">Display name.</span></span>|
|<span data-ttu-id="02231-113">oldValue</span><span class="sxs-lookup"><span data-stu-id="02231-113">oldValue</span></span>|<span data-ttu-id="02231-114">String</span><span class="sxs-lookup"><span data-stu-id="02231-114">String</span></span>|<span data-ttu-id="02231-115">旧值。</span><span class="sxs-lookup"><span data-stu-id="02231-115">Old value.</span></span>|
|<span data-ttu-id="02231-116">NewValue</span><span class="sxs-lookup"><span data-stu-id="02231-116">newValue</span></span>|<span data-ttu-id="02231-117">String</span><span class="sxs-lookup"><span data-stu-id="02231-117">String</span></span>|<span data-ttu-id="02231-118">新值。</span><span class="sxs-lookup"><span data-stu-id="02231-118">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="02231-119">关系</span><span class="sxs-lookup"><span data-stu-id="02231-119">Relationships</span></span>
<span data-ttu-id="02231-120">无</span><span class="sxs-lookup"><span data-stu-id="02231-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="02231-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="02231-121">JSON Representation</span></span>
<span data-ttu-id="02231-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="02231-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditProperty"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditProperty",
  "displayName": "String",
  "oldValue": "String",
  "newValue": "String"
}
```



