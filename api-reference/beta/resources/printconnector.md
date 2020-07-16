---
title: printConnector 资源类型
description: 表示已使用通用打印订阅注册的打印连接器。 PrintConnector 资源可用于查看连接器状态和更新属性。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 84c9625bd8d5a454100cab166676c1dcbcfd8d05
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142426"
---
# <a name="printconnector-resource-type"></a><span data-ttu-id="d2a3f-104">printConnector 资源类型</span><span class="sxs-lookup"><span data-stu-id="d2a3f-104">printConnector resource type</span></span>

<span data-ttu-id="d2a3f-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2a3f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2a3f-106">表示已使用通用打印订阅注册的打印连接器。</span><span class="sxs-lookup"><span data-stu-id="d2a3f-106">Represents a print connector that has been registered by using a Universal Print subscription.</span></span> <span data-ttu-id="d2a3f-107">PrintConnector 资源可用于查看连接器状态和更新属性。</span><span class="sxs-lookup"><span data-stu-id="d2a3f-107">The printConnector resource can be used to view connector status and update properties.</span></span>

## <a name="methods"></a><span data-ttu-id="d2a3f-108">方法</span><span class="sxs-lookup"><span data-stu-id="d2a3f-108">Methods</span></span>

| <span data-ttu-id="d2a3f-109">方法</span><span class="sxs-lookup"><span data-stu-id="d2a3f-109">Method</span></span>       | <span data-ttu-id="d2a3f-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d2a3f-110">Return Type</span></span> | <span data-ttu-id="d2a3f-111">说明</span><span class="sxs-lookup"><span data-stu-id="d2a3f-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d2a3f-112">获取连接器</span><span class="sxs-lookup"><span data-stu-id="d2a3f-112">Get connector</span></span>](../api/printconnector-get.md) | [<span data-ttu-id="d2a3f-113">printConnector</span><span class="sxs-lookup"><span data-stu-id="d2a3f-113">printConnector</span></span>](printconnector.md) | <span data-ttu-id="d2a3f-114">读取连接器对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d2a3f-114">Read the properties and relationships of the connector object.</span></span> |
| [<span data-ttu-id="d2a3f-115">更新连接器</span><span class="sxs-lookup"><span data-stu-id="d2a3f-115">Update connector</span></span>](../api/printconnector-update.md) | [<span data-ttu-id="d2a3f-116">printConnector</span><span class="sxs-lookup"><span data-stu-id="d2a3f-116">printConnector</span></span>](printconnector.md) | <span data-ttu-id="d2a3f-117">更新连接器对象。</span><span class="sxs-lookup"><span data-stu-id="d2a3f-117">Update the connector object.</span></span> |
| [<span data-ttu-id="d2a3f-118">删除连接器</span><span class="sxs-lookup"><span data-stu-id="d2a3f-118">Delete connector</span></span>](../api/printconnector-delete.md) | <span data-ttu-id="d2a3f-119">无</span><span class="sxs-lookup"><span data-stu-id="d2a3f-119">None</span></span> | <span data-ttu-id="d2a3f-120">从通用打印服务中注销连接器。</span><span class="sxs-lookup"><span data-stu-id="d2a3f-120">Unregister the connector from the Universal Print service.</span></span> |

## <a name="properties"></a><span data-ttu-id="d2a3f-121">属性</span><span class="sxs-lookup"><span data-stu-id="d2a3f-121">Properties</span></span>
| <span data-ttu-id="d2a3f-122">属性</span><span class="sxs-lookup"><span data-stu-id="d2a3f-122">Property</span></span>     | <span data-ttu-id="d2a3f-123">类型</span><span class="sxs-lookup"><span data-stu-id="d2a3f-123">Type</span></span>        | <span data-ttu-id="d2a3f-124">说明</span><span class="sxs-lookup"><span data-stu-id="d2a3f-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d2a3f-125">id</span><span class="sxs-lookup"><span data-stu-id="d2a3f-125">id</span></span>|<span data-ttu-id="d2a3f-126">String</span><span class="sxs-lookup"><span data-stu-id="d2a3f-126">String</span></span>| <span data-ttu-id="d2a3f-127">只读。</span><span class="sxs-lookup"><span data-stu-id="d2a3f-127">Read-only.</span></span>|
|<span data-ttu-id="d2a3f-128">name</span><span class="sxs-lookup"><span data-stu-id="d2a3f-128">name</span></span>|<span data-ttu-id="d2a3f-129">String</span><span class="sxs-lookup"><span data-stu-id="d2a3f-129">String</span></span>|<span data-ttu-id="d2a3f-130">连接器的名称。</span><span class="sxs-lookup"><span data-stu-id="d2a3f-130">The name of the connector.</span></span>|
|<span data-ttu-id="d2a3f-131">fullyQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="d2a3f-131">fullyQualifiedDomainName</span></span>|<span data-ttu-id="d2a3f-132">String</span><span class="sxs-lookup"><span data-stu-id="d2a3f-132">String</span></span>|<span data-ttu-id="d2a3f-133">连接器计算机的主机名。</span><span class="sxs-lookup"><span data-stu-id="d2a3f-133">The connector machine's hostname.</span></span>|
|<span data-ttu-id="d2a3f-134">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="d2a3f-134">operatingSystem</span></span>|<span data-ttu-id="d2a3f-135">String</span><span class="sxs-lookup"><span data-stu-id="d2a3f-135">String</span></span>|<span data-ttu-id="d2a3f-136">连接器计算机的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="d2a3f-136">The connector machine's operating system version.</span></span>|
|<span data-ttu-id="d2a3f-137">appVersion</span><span class="sxs-lookup"><span data-stu-id="d2a3f-137">appVersion</span></span>|<span data-ttu-id="d2a3f-138">String</span><span class="sxs-lookup"><span data-stu-id="d2a3f-138">String</span></span>|<span data-ttu-id="d2a3f-139">连接器的版本。</span><span class="sxs-lookup"><span data-stu-id="d2a3f-139">The connector's version.</span></span>|
|<span data-ttu-id="d2a3f-140">deviceHealth</span><span class="sxs-lookup"><span data-stu-id="d2a3f-140">deviceHealth</span></span>|[<span data-ttu-id="d2a3f-141">deviceHealth</span><span class="sxs-lookup"><span data-stu-id="d2a3f-141">deviceHealth</span></span>](devicehealth.md)|<span data-ttu-id="d2a3f-142">连接器的设备运行状况。</span><span class="sxs-lookup"><span data-stu-id="d2a3f-142">The connector's device health.</span></span>|
|<span data-ttu-id="d2a3f-143">位置</span><span class="sxs-lookup"><span data-stu-id="d2a3f-143">location</span></span>|[<span data-ttu-id="d2a3f-144">printerLocation</span><span class="sxs-lookup"><span data-stu-id="d2a3f-144">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="d2a3f-145">连接器的物理位置和/或组织位置。</span><span class="sxs-lookup"><span data-stu-id="d2a3f-145">The physical and/or organizational location of the connector.</span></span>|
|<span data-ttu-id="d2a3f-146">registeredDateTime</span><span class="sxs-lookup"><span data-stu-id="d2a3f-146">registeredDateTime</span></span>|<span data-ttu-id="d2a3f-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2a3f-147">DateTimeOffset</span></span>|<span data-ttu-id="d2a3f-148">注册连接器时的 DateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="d2a3f-148">The DateTimeOffset when the connector was registered.</span></span>|
|<span data-ttu-id="d2a3f-149">registeredBy</span><span class="sxs-lookup"><span data-stu-id="d2a3f-149">registeredBy</span></span>|[<span data-ttu-id="d2a3f-150">userIdentity</span><span class="sxs-lookup"><span data-stu-id="d2a3f-150">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="d2a3f-151">注册了连接器的用户。</span><span class="sxs-lookup"><span data-stu-id="d2a3f-151">The user who registered the connector.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d2a3f-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d2a3f-152">JSON representation</span></span>

<span data-ttu-id="d2a3f-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2a3f-153">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printConnector"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "fullyQualifiedDomainName": "String",
  "operatingSystem": "String",
  "appVersion": "String",
  "deviceHealth": {"@odata.type": "microsoft.graph.deviceHealth"},
  "location": {"@odata.type": "microsoft.graph.printerLocation"},
  "registeredDateTime": "String (timestamp)",
  "registeredBy": {"@odata.type": "microsoft.graph.userIdentity"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printConnector resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
