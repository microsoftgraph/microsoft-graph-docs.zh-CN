---
title: cloudPcUserRoleScopeTagInfo 资源类型
description: 表示具有标识和显示名称范围标记信息。
author: ecmadao
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 61df383dca51ec2494eb10b745bc227bcfc5d9b8
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211213"
---
# <a name="cloudpcuserrolescopetaginfo-resource-type"></a><span data-ttu-id="5fb1e-103">cloudPcUserRoleScopeTagInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="5fb1e-103">cloudPcUserRoleScopeTagInfo resource type</span></span>

<span data-ttu-id="5fb1e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5fb1e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5fb1e-105">表示具有标识和显示名称范围标记信息。</span><span class="sxs-lookup"><span data-stu-id="5fb1e-105">Represents the scope tag info with display name and identity.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="5fb1e-106">属性</span><span class="sxs-lookup"><span data-stu-id="5fb1e-106">Properties</span></span>
|<span data-ttu-id="5fb1e-107">属性</span><span class="sxs-lookup"><span data-stu-id="5fb1e-107">Property</span></span>|<span data-ttu-id="5fb1e-108">类型</span><span class="sxs-lookup"><span data-stu-id="5fb1e-108">Type</span></span>|<span data-ttu-id="5fb1e-109">说明</span><span class="sxs-lookup"><span data-stu-id="5fb1e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5fb1e-110">displayName</span><span class="sxs-lookup"><span data-stu-id="5fb1e-110">displayName</span></span>|<span data-ttu-id="5fb1e-111">String</span><span class="sxs-lookup"><span data-stu-id="5fb1e-111">String</span></span>|<span data-ttu-id="5fb1e-112">范围标记显示名称。</span><span class="sxs-lookup"><span data-stu-id="5fb1e-112">Scope tag display name.</span></span>|
|<span data-ttu-id="5fb1e-113">roleScopeTagId</span><span class="sxs-lookup"><span data-stu-id="5fb1e-113">roleScopeTagId</span></span>|<span data-ttu-id="5fb1e-114">String</span><span class="sxs-lookup"><span data-stu-id="5fb1e-114">String</span></span>|<span data-ttu-id="5fb1e-115">范围标记 ID。</span><span class="sxs-lookup"><span data-stu-id="5fb1e-115">Scope tag ID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5fb1e-116">关系</span><span class="sxs-lookup"><span data-stu-id="5fb1e-116">Relationships</span></span>

<span data-ttu-id="5fb1e-117">无</span><span class="sxs-lookup"><span data-stu-id="5fb1e-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5fb1e-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5fb1e-118">JSON Representation</span></span>
<span data-ttu-id="5fb1e-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5fb1e-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcUserRoleScopeTagInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcUserRoleScopeTagInfo",
  "displayName": "String",
  "roleScopeTagId": "String"
}
```