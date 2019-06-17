---
title: extendedKeyUsage 资源类型
description: 自定义扩展密钥用法定义
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9eb9a02c8f403bf4ee29fc28622ab06f592c870b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34982516"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="dd763-103">extendedKeyUsage 资源类型</span><span class="sxs-lookup"><span data-stu-id="dd763-103">extendedKeyUsage resource type</span></span>

> <span data-ttu-id="dd763-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dd763-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd763-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dd763-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd763-106">自定义扩展密钥用法定义</span><span class="sxs-lookup"><span data-stu-id="dd763-106">Custom Extended Key Usage definition</span></span>

## <a name="properties"></a><span data-ttu-id="dd763-107">属性</span><span class="sxs-lookup"><span data-stu-id="dd763-107">Properties</span></span>
|<span data-ttu-id="dd763-108">属性</span><span class="sxs-lookup"><span data-stu-id="dd763-108">Property</span></span>|<span data-ttu-id="dd763-109">类型</span><span class="sxs-lookup"><span data-stu-id="dd763-109">Type</span></span>|<span data-ttu-id="dd763-110">说明</span><span class="sxs-lookup"><span data-stu-id="dd763-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd763-111">name</span><span class="sxs-lookup"><span data-stu-id="dd763-111">name</span></span>|<span data-ttu-id="dd763-112">String</span><span class="sxs-lookup"><span data-stu-id="dd763-112">String</span></span>|<span data-ttu-id="dd763-113">扩展密钥用法名称</span><span class="sxs-lookup"><span data-stu-id="dd763-113">Extended Key Usage Name</span></span>|
|<span data-ttu-id="dd763-114">objectIdentifier</span><span class="sxs-lookup"><span data-stu-id="dd763-114">objectIdentifier</span></span>|<span data-ttu-id="dd763-115">String</span><span class="sxs-lookup"><span data-stu-id="dd763-115">String</span></span>|<span data-ttu-id="dd763-116">扩展密钥用法对象标识符</span><span class="sxs-lookup"><span data-stu-id="dd763-116">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd763-117">关系</span><span class="sxs-lookup"><span data-stu-id="dd763-117">Relationships</span></span>
<span data-ttu-id="dd763-118">无</span><span class="sxs-lookup"><span data-stu-id="dd763-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dd763-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dd763-119">JSON Representation</span></span>
<span data-ttu-id="dd763-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd763-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.extendedKeyUsage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.extendedKeyUsage",
  "name": "String",
  "objectIdentifier": "String"
}
```





