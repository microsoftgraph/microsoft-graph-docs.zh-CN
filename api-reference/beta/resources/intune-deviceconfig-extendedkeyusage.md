---
title: extendedKeyUsage 资源类型
description: 自定义扩展密钥用法定义
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 89b97b7061e34fbb83b33c7ec0a9e626d7eb5a5e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696172"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="8c80a-103">extendedKeyUsage 资源类型</span><span class="sxs-lookup"><span data-stu-id="8c80a-103">extendedKeyUsage resource type</span></span>

<span data-ttu-id="8c80a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c80a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8c80a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8c80a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c80a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8c80a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c80a-107">自定义扩展密钥用法定义</span><span class="sxs-lookup"><span data-stu-id="8c80a-107">Custom Extended Key Usage definition</span></span>

## <a name="properties"></a><span data-ttu-id="8c80a-108">属性</span><span class="sxs-lookup"><span data-stu-id="8c80a-108">Properties</span></span>
|<span data-ttu-id="8c80a-109">属性</span><span class="sxs-lookup"><span data-stu-id="8c80a-109">Property</span></span>|<span data-ttu-id="8c80a-110">类型</span><span class="sxs-lookup"><span data-stu-id="8c80a-110">Type</span></span>|<span data-ttu-id="8c80a-111">说明</span><span class="sxs-lookup"><span data-stu-id="8c80a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c80a-112">name</span><span class="sxs-lookup"><span data-stu-id="8c80a-112">name</span></span>|<span data-ttu-id="8c80a-113">String</span><span class="sxs-lookup"><span data-stu-id="8c80a-113">String</span></span>|<span data-ttu-id="8c80a-114">扩展密钥用法名称</span><span class="sxs-lookup"><span data-stu-id="8c80a-114">Extended Key Usage Name</span></span>|
|<span data-ttu-id="8c80a-115">objectIdentifier</span><span class="sxs-lookup"><span data-stu-id="8c80a-115">objectIdentifier</span></span>|<span data-ttu-id="8c80a-116">String</span><span class="sxs-lookup"><span data-stu-id="8c80a-116">String</span></span>|<span data-ttu-id="8c80a-117">扩展密钥用法对象标识符</span><span class="sxs-lookup"><span data-stu-id="8c80a-117">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c80a-118">关系</span><span class="sxs-lookup"><span data-stu-id="8c80a-118">Relationships</span></span>
<span data-ttu-id="8c80a-119">无</span><span class="sxs-lookup"><span data-stu-id="8c80a-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c80a-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8c80a-120">JSON Representation</span></span>
<span data-ttu-id="8c80a-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c80a-121">Here is a JSON representation of the resource.</span></span>
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





