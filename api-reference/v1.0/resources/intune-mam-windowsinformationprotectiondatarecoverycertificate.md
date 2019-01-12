---
title: windowsInformationProtectionDataRecoveryCertificate 资源类型
description: Windows 信息保护 DataRecoveryCertificate
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2a40fc3ab500fe6aa2a5b0f373c78524444b5bd1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971856"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="ea7b7-103">windowsInformationProtectionDataRecoveryCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="ea7b7-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="ea7b7-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ea7b7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea7b7-105">Windows 信息保护 DataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="ea7b7-105">Windows Information Protection DataRecoveryCertificate</span></span>
## <a name="properties"></a><span data-ttu-id="ea7b7-106">属性</span><span class="sxs-lookup"><span data-stu-id="ea7b7-106">Properties</span></span>
|<span data-ttu-id="ea7b7-107">属性</span><span class="sxs-lookup"><span data-stu-id="ea7b7-107">Property</span></span>|<span data-ttu-id="ea7b7-108">类型</span><span class="sxs-lookup"><span data-stu-id="ea7b7-108">Type</span></span>|<span data-ttu-id="ea7b7-109">说明</span><span class="sxs-lookup"><span data-stu-id="ea7b7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea7b7-110">SubjectName</span><span class="sxs-lookup"><span data-stu-id="ea7b7-110">subjectName</span></span>|<span data-ttu-id="ea7b7-111">String</span><span class="sxs-lookup"><span data-stu-id="ea7b7-111">String</span></span>|<span data-ttu-id="ea7b7-112">数据恢复证书主题名称</span><span class="sxs-lookup"><span data-stu-id="ea7b7-112">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="ea7b7-113">description</span><span class="sxs-lookup"><span data-stu-id="ea7b7-113">description</span></span>|<span data-ttu-id="ea7b7-114">String</span><span class="sxs-lookup"><span data-stu-id="ea7b7-114">String</span></span>|<span data-ttu-id="ea7b7-115">数据恢复证书说明</span><span class="sxs-lookup"><span data-stu-id="ea7b7-115">Data recovery Certificate description</span></span>|
|<span data-ttu-id="ea7b7-116">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ea7b7-116">expirationDateTime</span></span>|<span data-ttu-id="ea7b7-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea7b7-117">DateTimeOffset</span></span>|<span data-ttu-id="ea7b7-118">数据恢复证书过期日期/时间</span><span class="sxs-lookup"><span data-stu-id="ea7b7-118">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="ea7b7-119">证书</span><span class="sxs-lookup"><span data-stu-id="ea7b7-119">certificate</span></span>|<span data-ttu-id="ea7b7-120">Binary</span><span class="sxs-lookup"><span data-stu-id="ea7b7-120">Binary</span></span>|<span data-ttu-id="ea7b7-121">数据恢复证书</span><span class="sxs-lookup"><span data-stu-id="ea7b7-121">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea7b7-122">关系</span><span class="sxs-lookup"><span data-stu-id="ea7b7-122">Relationships</span></span>
<span data-ttu-id="ea7b7-123">无</span><span class="sxs-lookup"><span data-stu-id="ea7b7-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ea7b7-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ea7b7-124">JSON Representation</span></span>
<span data-ttu-id="ea7b7-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ea7b7-125">Here is a JSON representation of the resource.</span></span>
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



