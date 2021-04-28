---
title: updatableAssetError 资源类型
description: 表示阻止部署服务在更新管理中注册 azureADDevice 或将内容部署到设备的错误的抽象类型
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 4d4375be68aea6dd4cb27c7ae8b78aaf86a2edf1
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067301"
---
# <a name="updatableasseterror-resource-type"></a><span data-ttu-id="edc2a-103">updatableAssetError 资源类型</span><span class="sxs-lookup"><span data-stu-id="edc2a-103">updatableAssetError resource type</span></span>

<span data-ttu-id="edc2a-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="edc2a-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edc2a-105">表示阻止部署服务在更新管理中注册 [azureADDevice](../resources/windowsupdates-azureaddevice.md) 或将内容部署到设备的错误的抽象类型。</span><span class="sxs-lookup"><span data-stu-id="edc2a-105">An abstract type that represents an error which prevents the deployment service from enrolling an [azureADDevice](../resources/windowsupdates-azureaddevice.md) in update management, or deploying content to the device.</span></span> 

<span data-ttu-id="edc2a-106">所有可更新资源错误都是派生类型的 [azureADDeviceRegistrationError](../resources/windowsupdates-azureaddeviceregistrationerror.md)。</span><span class="sxs-lookup"><span data-stu-id="edc2a-106">All updatable asset errors are of the derived type, [azureADDeviceRegistrationError](../resources/windowsupdates-azureaddeviceregistrationerror.md).</span></span>


## <a name="properties"></a><span data-ttu-id="edc2a-107">属性</span><span class="sxs-lookup"><span data-stu-id="edc2a-107">Properties</span></span>
<span data-ttu-id="edc2a-108">无。</span><span class="sxs-lookup"><span data-stu-id="edc2a-108">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="edc2a-109">关系</span><span class="sxs-lookup"><span data-stu-id="edc2a-109">Relationships</span></span>
<span data-ttu-id="edc2a-110">无。</span><span class="sxs-lookup"><span data-stu-id="edc2a-110">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="edc2a-111">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="edc2a-111">JSON representation</span></span>
<span data-ttu-id="edc2a-112">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="edc2a-112">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.updatableAssetError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetError"
}
```

