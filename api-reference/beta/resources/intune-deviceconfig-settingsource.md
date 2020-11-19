---
title: settingSource 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5f0ebdabfbcb77a650580e92aaa3af14e2e9035a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49293750"
---
# <a name="settingsource-resource-type"></a><span data-ttu-id="24181-103">settingSource 资源类型</span><span class="sxs-lookup"><span data-stu-id="24181-103">settingSource resource type</span></span>

<span data-ttu-id="24181-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24181-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="24181-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="24181-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24181-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="24181-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24181-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="24181-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="24181-108">属性</span><span class="sxs-lookup"><span data-stu-id="24181-108">Properties</span></span>
|<span data-ttu-id="24181-109">属性</span><span class="sxs-lookup"><span data-stu-id="24181-109">Property</span></span>|<span data-ttu-id="24181-110">类型</span><span class="sxs-lookup"><span data-stu-id="24181-110">Type</span></span>|<span data-ttu-id="24181-111">说明</span><span class="sxs-lookup"><span data-stu-id="24181-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24181-112">id</span><span class="sxs-lookup"><span data-stu-id="24181-112">id</span></span>|<span data-ttu-id="24181-113">字符串</span><span class="sxs-lookup"><span data-stu-id="24181-113">String</span></span>|<span data-ttu-id="24181-114">尚未记录</span><span class="sxs-lookup"><span data-stu-id="24181-114">Not yet documented</span></span>|
|<span data-ttu-id="24181-115">displayName</span><span class="sxs-lookup"><span data-stu-id="24181-115">displayName</span></span>|<span data-ttu-id="24181-116">字符串</span><span class="sxs-lookup"><span data-stu-id="24181-116">String</span></span>|<span data-ttu-id="24181-117">尚未记录</span><span class="sxs-lookup"><span data-stu-id="24181-117">Not yet documented</span></span>|
|<span data-ttu-id="24181-118">sourceType</span><span class="sxs-lookup"><span data-stu-id="24181-118">sourceType</span></span>|[<span data-ttu-id="24181-119">settingSourceType</span><span class="sxs-lookup"><span data-stu-id="24181-119">settingSourceType</span></span>](../resources/intune-shared-settingsourcetype.md)|<span data-ttu-id="24181-120">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="24181-120">Not yet documented.</span></span> <span data-ttu-id="24181-121">可取值为：`deviceConfiguration`、`deviceIntent`。</span><span class="sxs-lookup"><span data-stu-id="24181-121">Possible values are: `deviceConfiguration`, `deviceIntent`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="24181-122">关系</span><span class="sxs-lookup"><span data-stu-id="24181-122">Relationships</span></span>
<span data-ttu-id="24181-123">无</span><span class="sxs-lookup"><span data-stu-id="24181-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="24181-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="24181-124">JSON Representation</span></span>
<span data-ttu-id="24181-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="24181-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.settingSource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.settingSource",
  "id": "String (identifier)",
  "displayName": "String",
  "sourceType": "String"
}
```




