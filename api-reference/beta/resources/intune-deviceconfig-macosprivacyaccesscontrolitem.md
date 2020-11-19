---
title: macOSPrivacyAccessControlItem 资源类型
description: 表示每个进程的隐私首选项。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fc290e76b7f0f1988f65e44a107b73c8188704df
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49294149"
---
# <a name="macosprivacyaccesscontrolitem-resource-type"></a>macOSPrivacyAccessControlItem 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示每个进程的隐私首选项。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|字符串|应用程序、进程或可执行文件的显示名称。|
|标识符|字符串|应用程序、进程或可执行文件的捆绑包 ID 或路径。|
|identifierType|[macOSProcessIdentifierType](../resources/intune-deviceconfig-macosprocessidentifiertype.md)|捆绑包 ID 用于标识应用程序。 路径用于标识进程或可执行文件。 可取值为：`bundleID`、`path`。|
|codeRequirement|字符串|输入可通过终端应用中的命令 "codesign – r –" 获取的代码要求。 包含 "=>" 后面的所有内容。|
|staticCodeValidation|Boolean|以静态方式验证代码要求。 如果进程使其动态代码签名失效，请使用此设置。|
|blockCamera|Boolean|阻止对相机应用的访问。|
|blockMicrophone|Boolean|阻止对麦克风的访问。|
|blockScreenCapture|Boolean|阻止应用捕获系统显示内容。 需要 macOS 10.15 或更高版本。|
|blockListenEvent|Boolean|阻止应用程序或进程侦听来自输入设备（如鼠标、键盘和 trackpad）的事件。需要 macOS 10.15 或更高版本。|
|speechRecognition|[启用](../resources/intune-shared-enablement.md)|允许或阻止对系统语音识别功能的访问。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|工具|[启用](../resources/intune-shared-enablement.md)|允许应用或进程通过辅助功能子系统控制 Mac。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|addressBook|[启用](../resources/intune-shared-enablement.md)|允许或阻止对联系人管理的联系人信息的访问。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|calendar|[启用](../resources/intune-shared-enablement.md)|允许或阻止对日历管理的事件信息的访问。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|提醒|[启用](../resources/intune-shared-enablement.md)|允许或阻止对由提醒管理的信息的访问。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|photos|[启用](../resources/intune-shared-enablement.md)|允许或阻止对照片管理的图像的访问。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|mediaLibrary|[启用](../resources/intune-shared-enablement.md)|允许或阻止对音乐和媒体库的访问。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|fileProviderPresence|[启用](../resources/intune-shared-enablement.md)|允许应用或进程访问由另一个应用程序的文件提供程序扩展管理的文件。 需要 macOS 10.15 或更高版本。 . 可取值为：`notConfigured`、`enabled`、`disabled`。|
|systemPolicyAllFiles|[启用](../resources/intune-shared-enablement.md)|控制对设备上所有受保护文件的访问。 文件可能位于电子邮件、邮件、应用程序和管理设置等位置。 请谨慎应用此设置。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|systemPolicySystemAdminFiles|[启用](../resources/intune-shared-enablement.md)|允许应用或进程访问在系统管理中使用的文件。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|systemPolicyDesktopFolder|[启用](../resources/intune-shared-enablement.md)|允许或阻止对桌面文件夹的访问。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|systemPolicyDocumentsFolder|[启用](../resources/intune-shared-enablement.md)|允许或阻止对文档文件夹的访问。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|systemPolicyDownloadsFolder|[启用](../resources/intune-shared-enablement.md)|允许或阻止对下载文件夹的访问。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|systemPolicyNetworkVolumes|[启用](../resources/intune-shared-enablement.md)|允许或阻止对网络卷的访问。 需要 macOS 10.15 或更高版本。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|systemPolicyRemovableVolumes|[启用](../resources/intune-shared-enablement.md)|控制对设备上可移动卷（如外部硬盘驱动器）的访问。 需要 macOS 10.15 或更高版本。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|postEvent|[启用](../resources/intune-shared-enablement.md)|控制对 CoreGraphics Api 的访问，这些 Api 用于将 CGEvents 发送到系统事件流。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|appleEventsAllowedReceivers|[macOSAppleEventReceiver](../resources/intune-deviceconfig-macosappleeventreceiver.md) 集合|允许或拒绝将受限制的 Apple 事件发送到另一个应用程序或进程的应用程序或进程。 您将需要知道接收应用程序或进程的标识符、标识符类型和代码要求。 该集合最多可包含 500 个元素。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSPrivacyAccessControlItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSPrivacyAccessControlItem",
  "displayName": "String",
  "identifier": "String",
  "identifierType": "String",
  "codeRequirement": "String",
  "staticCodeValidation": true,
  "blockCamera": true,
  "blockMicrophone": true,
  "blockScreenCapture": true,
  "blockListenEvent": true,
  "speechRecognition": "String",
  "accessibility": "String",
  "addressBook": "String",
  "calendar": "String",
  "reminders": "String",
  "photos": "String",
  "mediaLibrary": "String",
  "fileProviderPresence": "String",
  "systemPolicyAllFiles": "String",
  "systemPolicySystemAdminFiles": "String",
  "systemPolicyDesktopFolder": "String",
  "systemPolicyDocumentsFolder": "String",
  "systemPolicyDownloadsFolder": "String",
  "systemPolicyNetworkVolumes": "String",
  "systemPolicyRemovableVolumes": "String",
  "postEvent": "String",
  "appleEventsAllowedReceivers": [
    {
      "@odata.type": "microsoft.graph.macOSAppleEventReceiver",
      "codeRequirement": "String",
      "identifier": "String",
      "identifierType": "String",
      "allowed": true
    }
  ]
}
```




