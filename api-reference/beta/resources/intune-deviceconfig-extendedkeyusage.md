---
title: extendedKeyUsage 资源类型
description: 自定义扩展密钥用法定义
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d02154b9513e1ef3edac8cf823bd718d3e356691
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325580"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="0c2f3-103">extendedKeyUsage 资源类型</span><span class="sxs-lookup"><span data-stu-id="0c2f3-103">extendedKeyUsage resource type</span></span>

> <span data-ttu-id="0c2f3-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0c2f3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c2f3-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0c2f3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c2f3-106">自定义扩展密钥用法定义</span><span class="sxs-lookup"><span data-stu-id="0c2f3-106">Custom Extended Key Usage definition</span></span>

## <a name="properties"></a><span data-ttu-id="0c2f3-107">属性</span><span class="sxs-lookup"><span data-stu-id="0c2f3-107">Properties</span></span>
|<span data-ttu-id="0c2f3-108">属性</span><span class="sxs-lookup"><span data-stu-id="0c2f3-108">Property</span></span>|<span data-ttu-id="0c2f3-109">类型</span><span class="sxs-lookup"><span data-stu-id="0c2f3-109">Type</span></span>|<span data-ttu-id="0c2f3-110">说明</span><span class="sxs-lookup"><span data-stu-id="0c2f3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c2f3-111">name</span><span class="sxs-lookup"><span data-stu-id="0c2f3-111">name</span></span>|<span data-ttu-id="0c2f3-112">String</span><span class="sxs-lookup"><span data-stu-id="0c2f3-112">String</span></span>|<span data-ttu-id="0c2f3-113">扩展密钥用法名称</span><span class="sxs-lookup"><span data-stu-id="0c2f3-113">Extended Key Usage Name</span></span>|
|<span data-ttu-id="0c2f3-114">objectIdentifier</span><span class="sxs-lookup"><span data-stu-id="0c2f3-114">objectIdentifier</span></span>|<span data-ttu-id="0c2f3-115">String</span><span class="sxs-lookup"><span data-stu-id="0c2f3-115">String</span></span>|<span data-ttu-id="0c2f3-116">扩展密钥用法对象标识符</span><span class="sxs-lookup"><span data-stu-id="0c2f3-116">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c2f3-117">关系</span><span class="sxs-lookup"><span data-stu-id="0c2f3-117">Relationships</span></span>
<span data-ttu-id="0c2f3-118">无</span><span class="sxs-lookup"><span data-stu-id="0c2f3-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c2f3-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0c2f3-119">JSON Representation</span></span>
<span data-ttu-id="0c2f3-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0c2f3-120">Here is a JSON representation of the resource.</span></span>
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



