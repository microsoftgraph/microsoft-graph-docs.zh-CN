---
title: deviceLogCollectionRequest 资源类型
description: Windows 日志集合请求实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f48e8511f7cbce95e15b1816831a471207c1558a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49299329"
---
# <a name="devicelogcollectionrequest-resource-type"></a><span data-ttu-id="efa2c-103">deviceLogCollectionRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="efa2c-103">deviceLogCollectionRequest resource type</span></span>

<span data-ttu-id="efa2c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efa2c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="efa2c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="efa2c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="efa2c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="efa2c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efa2c-107">Windows 日志集合请求实体。</span><span class="sxs-lookup"><span data-stu-id="efa2c-107">Windows Log Collection request entity.</span></span>

## <a name="properties"></a><span data-ttu-id="efa2c-108">属性</span><span class="sxs-lookup"><span data-stu-id="efa2c-108">Properties</span></span>
|<span data-ttu-id="efa2c-109">属性</span><span class="sxs-lookup"><span data-stu-id="efa2c-109">Property</span></span>|<span data-ttu-id="efa2c-110">类型</span><span class="sxs-lookup"><span data-stu-id="efa2c-110">Type</span></span>|<span data-ttu-id="efa2c-111">说明</span><span class="sxs-lookup"><span data-stu-id="efa2c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efa2c-112">id</span><span class="sxs-lookup"><span data-stu-id="efa2c-112">id</span></span>|<span data-ttu-id="efa2c-113">字符串</span><span class="sxs-lookup"><span data-stu-id="efa2c-113">String</span></span>|<span data-ttu-id="efa2c-114">唯一标识符</span><span class="sxs-lookup"><span data-stu-id="efa2c-114">The unique identifier</span></span>|
|<span data-ttu-id="efa2c-115">templateType</span><span class="sxs-lookup"><span data-stu-id="efa2c-115">templateType</span></span>|[<span data-ttu-id="efa2c-116">deviceLogCollectionTemplateType</span><span class="sxs-lookup"><span data-stu-id="efa2c-116">deviceLogCollectionTemplateType</span></span>](../resources/intune-devices-devicelogcollectiontemplatetype.md)|<span data-ttu-id="efa2c-117">与集合请求一起发送的模板类型。</span><span class="sxs-lookup"><span data-stu-id="efa2c-117">The template type that is sent with the collection request.</span></span> <span data-ttu-id="efa2c-118">可能的值是： `predefined` 。</span><span class="sxs-lookup"><span data-stu-id="efa2c-118">Possible values are: `predefined`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="efa2c-119">关系</span><span class="sxs-lookup"><span data-stu-id="efa2c-119">Relationships</span></span>
<span data-ttu-id="efa2c-120">无</span><span class="sxs-lookup"><span data-stu-id="efa2c-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="efa2c-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="efa2c-121">JSON Representation</span></span>
<span data-ttu-id="efa2c-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="efa2c-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceLogCollectionRequest"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceLogCollectionRequest",
  "id": "String (identifier)",
  "templateType": "String"
}
```




