---
title: extendedKeyUsage 资源类型
description: 自定义扩展密钥用法定义
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 36752e9a2f86e68bd4ada1a342dc174726a684c7
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946950"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="76c0e-103">extendedKeyUsage 资源类型</span><span class="sxs-lookup"><span data-stu-id="76c0e-103">extendedKeyUsage resource type</span></span>

> <span data-ttu-id="76c0e-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="76c0e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76c0e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="76c0e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76c0e-106">自定义扩展密钥用法定义</span><span class="sxs-lookup"><span data-stu-id="76c0e-106">Custom Extended Key Usage definition</span></span>

## <a name="properties"></a><span data-ttu-id="76c0e-107">属性</span><span class="sxs-lookup"><span data-stu-id="76c0e-107">Properties</span></span>
|<span data-ttu-id="76c0e-108">属性</span><span class="sxs-lookup"><span data-stu-id="76c0e-108">Property</span></span>|<span data-ttu-id="76c0e-109">类型</span><span class="sxs-lookup"><span data-stu-id="76c0e-109">Type</span></span>|<span data-ttu-id="76c0e-110">说明</span><span class="sxs-lookup"><span data-stu-id="76c0e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76c0e-111">name</span><span class="sxs-lookup"><span data-stu-id="76c0e-111">name</span></span>|<span data-ttu-id="76c0e-112">String</span><span class="sxs-lookup"><span data-stu-id="76c0e-112">String</span></span>|<span data-ttu-id="76c0e-113">扩展密钥用法名称</span><span class="sxs-lookup"><span data-stu-id="76c0e-113">Extended Key Usage Name</span></span>|
|<span data-ttu-id="76c0e-114">objectIdentifier</span><span class="sxs-lookup"><span data-stu-id="76c0e-114">objectIdentifier</span></span>|<span data-ttu-id="76c0e-115">String</span><span class="sxs-lookup"><span data-stu-id="76c0e-115">String</span></span>|<span data-ttu-id="76c0e-116">扩展密钥用法对象标识符</span><span class="sxs-lookup"><span data-stu-id="76c0e-116">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="76c0e-117">关系</span><span class="sxs-lookup"><span data-stu-id="76c0e-117">Relationships</span></span>
<span data-ttu-id="76c0e-118">无</span><span class="sxs-lookup"><span data-stu-id="76c0e-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="76c0e-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="76c0e-119">JSON Representation</span></span>
<span data-ttu-id="76c0e-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="76c0e-120">Here is a JSON representation of the resource.</span></span>
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




