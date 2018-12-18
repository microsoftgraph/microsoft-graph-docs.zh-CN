---
title: managementCertificateWithThumbprint 资源类型
description: 尚未记录
author: tfitzmac
ms.openlocfilehash: 03846890822cae02a2eb04fc058895992119c98a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348935"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="91d4a-103">managementCertificateWithThumbprint 资源类型</span><span class="sxs-lookup"><span data-stu-id="91d4a-103">managementCertificateWithThumbprint resource type</span></span>

> <span data-ttu-id="91d4a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="91d4a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91d4a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="91d4a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="91d4a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="91d4a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="91d4a-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="91d4a-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="91d4a-108">属性</span><span class="sxs-lookup"><span data-stu-id="91d4a-108">Properties</span></span>
|<span data-ttu-id="91d4a-109">属性</span><span class="sxs-lookup"><span data-stu-id="91d4a-109">Property</span></span>|<span data-ttu-id="91d4a-110">类型</span><span class="sxs-lookup"><span data-stu-id="91d4a-110">Type</span></span>|<span data-ttu-id="91d4a-111">说明</span><span class="sxs-lookup"><span data-stu-id="91d4a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91d4a-112">指纹</span><span class="sxs-lookup"><span data-stu-id="91d4a-112">thumbprint</span></span>|<span data-ttu-id="91d4a-113">字符串</span><span class="sxs-lookup"><span data-stu-id="91d4a-113">String</span></span>|<span data-ttu-id="91d4a-114">管理证书的指纹</span><span class="sxs-lookup"><span data-stu-id="91d4a-114">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="91d4a-115">certificate</span><span class="sxs-lookup"><span data-stu-id="91d4a-115">certificate</span></span>|<span data-ttu-id="91d4a-116">String</span><span class="sxs-lookup"><span data-stu-id="91d4a-116">String</span></span>|<span data-ttu-id="91d4a-117">Base 64 编码的管理证书</span><span class="sxs-lookup"><span data-stu-id="91d4a-117">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="91d4a-118">Relationships</span><span class="sxs-lookup"><span data-stu-id="91d4a-118">Relationships</span></span>
<span data-ttu-id="91d4a-119">无</span><span class="sxs-lookup"><span data-stu-id="91d4a-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="91d4a-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="91d4a-120">JSON Representation</span></span>
<span data-ttu-id="91d4a-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91d4a-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managementCertificateWithThumbprint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementCertificateWithThumbprint",
  "thumbprint": "String",
  "certificate": "String"
}
```





