---
title: windowsInformationProtectionDataRecoveryCertificate 资源类型
description: Windows 信息保护 DataRecoveryCertificate
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5e686ab1a6c1e586c8bd32c56d3480102503b4be
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976252"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="009ec-103">windowsInformationProtectionDataRecoveryCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="009ec-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="009ec-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="009ec-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="009ec-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="009ec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="009ec-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="009ec-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="009ec-107">Windows 信息保护 DataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="009ec-107">Windows Information Protection DataRecoveryCertificate</span></span>
## <a name="properties"></a><span data-ttu-id="009ec-108">属性</span><span class="sxs-lookup"><span data-stu-id="009ec-108">Properties</span></span>
|<span data-ttu-id="009ec-109">属性</span><span class="sxs-lookup"><span data-stu-id="009ec-109">Property</span></span>|<span data-ttu-id="009ec-110">类型</span><span class="sxs-lookup"><span data-stu-id="009ec-110">Type</span></span>|<span data-ttu-id="009ec-111">说明</span><span class="sxs-lookup"><span data-stu-id="009ec-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="009ec-112">SubjectName</span><span class="sxs-lookup"><span data-stu-id="009ec-112">subjectName</span></span>|<span data-ttu-id="009ec-113">String</span><span class="sxs-lookup"><span data-stu-id="009ec-113">String</span></span>|<span data-ttu-id="009ec-114">数据恢复证书主题名称</span><span class="sxs-lookup"><span data-stu-id="009ec-114">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="009ec-115">description</span><span class="sxs-lookup"><span data-stu-id="009ec-115">description</span></span>|<span data-ttu-id="009ec-116">String</span><span class="sxs-lookup"><span data-stu-id="009ec-116">String</span></span>|<span data-ttu-id="009ec-117">数据恢复证书说明</span><span class="sxs-lookup"><span data-stu-id="009ec-117">Data recovery Certificate description</span></span>|
|<span data-ttu-id="009ec-118">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="009ec-118">expirationDateTime</span></span>|<span data-ttu-id="009ec-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="009ec-119">DateTimeOffset</span></span>|<span data-ttu-id="009ec-120">数据恢复证书过期日期/时间</span><span class="sxs-lookup"><span data-stu-id="009ec-120">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="009ec-121">证书</span><span class="sxs-lookup"><span data-stu-id="009ec-121">certificate</span></span>|<span data-ttu-id="009ec-122">Binary</span><span class="sxs-lookup"><span data-stu-id="009ec-122">Binary</span></span>|<span data-ttu-id="009ec-123">数据恢复证书</span><span class="sxs-lookup"><span data-stu-id="009ec-123">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="009ec-124">关系</span><span class="sxs-lookup"><span data-stu-id="009ec-124">Relationships</span></span>
<span data-ttu-id="009ec-125">无</span><span class="sxs-lookup"><span data-stu-id="009ec-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="009ec-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="009ec-126">JSON Representation</span></span>
<span data-ttu-id="009ec-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="009ec-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
  "subjectName": "String",
  "description": "String",
  "expirationDateTime": "String (timestamp)",
  "certificate": "binary"
}
```





