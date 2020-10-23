---
title: roleScopeTagInfo 资源类型
description: 包含 Role Scope Tag 对象的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 003906982c875fa4a70ee99c029f7c49b73b9398
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706028"
---
# <a name="rolescopetaginfo-resource-type"></a><span data-ttu-id="cec1c-103">roleScopeTagInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="cec1c-103">roleScopeTagInfo resource type</span></span>

<span data-ttu-id="cec1c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cec1c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cec1c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cec1c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cec1c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cec1c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cec1c-107">包含 Role Scope Tag 对象的属性的类。</span><span class="sxs-lookup"><span data-stu-id="cec1c-107">A class containing the properties of Role Scope Tag Object.</span></span>

## <a name="properties"></a><span data-ttu-id="cec1c-108">属性</span><span class="sxs-lookup"><span data-stu-id="cec1c-108">Properties</span></span>
|<span data-ttu-id="cec1c-109">属性</span><span class="sxs-lookup"><span data-stu-id="cec1c-109">Property</span></span>|<span data-ttu-id="cec1c-110">类型</span><span class="sxs-lookup"><span data-stu-id="cec1c-110">Type</span></span>|<span data-ttu-id="cec1c-111">说明</span><span class="sxs-lookup"><span data-stu-id="cec1c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cec1c-112">displayName</span><span class="sxs-lookup"><span data-stu-id="cec1c-112">displayName</span></span>|<span data-ttu-id="cec1c-113">String</span><span class="sxs-lookup"><span data-stu-id="cec1c-113">String</span></span>|<span data-ttu-id="cec1c-114">范围标记显示名称。</span><span class="sxs-lookup"><span data-stu-id="cec1c-114">Scope Tag Display name.</span></span>|
|<span data-ttu-id="cec1c-115">roleScopeTagId</span><span class="sxs-lookup"><span data-stu-id="cec1c-115">roleScopeTagId</span></span>|<span data-ttu-id="cec1c-116">String</span><span class="sxs-lookup"><span data-stu-id="cec1c-116">String</span></span>|<span data-ttu-id="cec1c-117">范围标记 Id。</span><span class="sxs-lookup"><span data-stu-id="cec1c-117">Scope Tag Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cec1c-118">关系</span><span class="sxs-lookup"><span data-stu-id="cec1c-118">Relationships</span></span>
<span data-ttu-id="cec1c-119">无</span><span class="sxs-lookup"><span data-stu-id="cec1c-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cec1c-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cec1c-120">JSON Representation</span></span>
<span data-ttu-id="cec1c-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cec1c-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.roleScopeTagInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleScopeTagInfo",
  "displayName": "String",
  "roleScopeTagId": "String"
}
```





