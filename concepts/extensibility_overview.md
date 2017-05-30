# <a name="add-custom-data-to-resources-using-extensions"></a>使用扩展向资源添加自定义数据

Microsoft Graph 提供单一 API 终结点，让你可以通过大量资源（例如[用户](../api-reference/v1.0/resources/user.md)和[邮件](../api-reference/v1.0/resources/message.md)）访问以用户为中心的丰富的数据和见解。现在有一种方法可以让你使用自己的应用程序数据**扩展** Microsoft Graph。无需外部数据存储即可以向 Microsoft Graph 资源添加自定义属性。例如，你可能决定通过扩展**用户**资源来使应用保持在轻量级并将应用特定的用户配置文件数据存储在 Microsoft Graph 中。或者，你可以保留应用的现有用户配置文件存储，并只需向**用户**资源添加特定于应用的存储标识符。

Microsoft Graph 提供两种类型的扩展。选择最适合应用程序需求的扩展类型：

*  **开放扩展**：开发人员入门的良好方法。
*  **架构扩展**：对于那些关心存储类型化数据，使其架构可发现和可共享，能够进行筛选以及将来能够执行输入数据验证和授权的开发人员而言，这是一种更通用的机制。

>**重要说明：**不能使用扩展存储敏感的个人身份信息，例如帐户凭据、政府标识号、持卡人数据、财务帐户数据、医疗保健信息或敏感的背景信息。

## <a name="supported-resources"></a>支持的资源

下表显示了当前支持的开放扩展和架构扩展，以及它们是处于一般可用性（GA，/v1.0 和 /beta 端点）还是仅处于预览状态（/beta 端点）。 

| 资源 | 开放扩展 | 架构扩展 |
|---------------|-------|-------|
| [管理单元](../api-reference/beta/resources/administrativeunit.md) | 仅供预览 | 仅供预览 |
|  [日历事件](../api-reference/v1.0/resources/event.md) | GA | GA |
|  [设备](../api-reference/v1.0/resources/device.md) | GA | GA |
|  [组](../api-reference/v1.0/resources/group.md) | GA | GA |
|  [组日历事件](../api-reference/v1.0/resources/event.md) | GA | GA |
|  [组对话帖子](../api-reference/v1.0/resources/post.md) | GA | GA |
|  [邮件](../api-reference/v1.0/resources/message.md) | GA | GA |
|  [组织](../api-reference/v1.0/resources/organization.md) | GA | GA |
|  [个人联系人](../api-reference/v1.0/resources/contact.md)| GA | GA |
|  [用户](../api-reference/v1.0/resources/user.md) | GA | GA |

使用工作帐户或学校帐户登录时，可以对所有这些资源使用扩展。此外，使用个人帐户登录时，可以对这些资源使用扩展 - **事件**、**帖子**、**组**、**邮件**、**联系人**和**用户**。 

## <a name="open-extensions"></a>开放扩展

[开放扩展](../api-reference/v1.0/resources/opentypeextension.md)（以前称为 Office 365 数据扩展）是提供灵活方法将非类型化应用数据直接添加到资源实例的[开放类型](http://www.odata.org/getting-started/advanced-tutorial/#openType)。 

开放扩展及其自定义数据可通过资源实例的 **扩展**导航属性访问。**extensionName** 属性是开放扩展中唯一的预定义可写属性。创建开放扩展时，必须为 **extensionName** 属性分配一个在租户内是唯一的名称。实现此目的的一种方法是使用反向域名名称系统 (DNS) 格式，该格式取决于你拥有的域，例如 `Com.Contoso.ContactInfo`。请勿在扩展名中使用 Microsoft 域（`Com.Microsoft` 或 `Com.OnMicrosoft`）。

只需使用同一个操作即可在资源实例中[创建开放扩展](../api-reference/v1.0/api/opentypeextension_post_opentypeextension.md)并将自定义数据存储到其中（请注意[下面的已知限制](known_issues.md#extensions)，了解受支持的部分资源）。随后可以[读取](../api-reference/v1.0/api/opentypeextension_get.md)、[更新](../api-reference/v1.0/api/opentypeextension_update.md)或[删除](../api-reference/v1.0/api/opentypeextension_delete.md)扩展及其数据。

开放扩展示例：[使用开放扩展向用户添加自定义数据](extensibility_open_users.md)

## <a name="schema-extensions"></a>架构扩展

通过[架构扩展](../api-reference/v1.0/resources/schemaextension.md)可以定义一个架构并使用它来扩展资源类型。首先创建架构扩展定义。然后，利用它通过强类型自定义数据扩展资源实例。此外，可以控制架构扩展的[状态](#schema-extensions-lifecycle)并使其可被其他应用发现。反之，这些应用可以将此扩展用于他们的数据，并在此基础上生成进一步的体验。

在创建架构扩展定义时，你必须提供其 **id** 的唯一名称。提供两个命名选项：

- 如果已经有通过租户验证的虚拟 `.com` 域，则可以使用域名和架构名称来定义一个唯一名称，采用以下格式：\{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}。例如，如果虚域是 contoso.com，则可以定义 `contoso_mySchema` 的 **id**。这是首选选项。
- 如果没有验证的虚域，则可以只设置架构名称的 **id**（不带域名称前缀），例如，`mySchema`。根据所提供的名称，Microsoft Graph 将为你分配一个字符串 ID，采用以下格式：ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}。例如，`extkvbmkofy_mySchema`。

将在 **id** 中看到用作复杂类型名称的此唯一名称，该复杂类型将在扩展的资源实例上存储自定义数据。 

与开放类型不同，管理架构扩展定义（[列出](../api-reference/v1.0/api/schemaextension_list.md)、[创建](../api-reference/v1.0/api/schemaextension_post_schemaextensions.md)、[获取](../api-reference/v1.0/api/schemaextension_get.md)、[更新](../api-reference/v1.0/api/schemaextension_update.md)及[删除](../api-reference/v1.0/api/schemaextension_delete.md)）和管理其数据（添加、获取、更新及删除数据）是独立的 API 操作集。 

由于架构扩展可作为复杂类型在目标资源的实例中访问，因此可以使用以下方法对架构扩展中的自定义数据执行 CRUD 操作：

- 创建新的资源实例时，使用资源 `POST` 方法指定自定义数据。
- 使用资源 `GET` 方法读取自定义数据。
- 使用资源 `PATCH` 方法添加或更新现有资源实例中的自定义数据。
- 使用资源 `PATCH` 方法将复杂类型设置为 NULL，以删除资源实例中的自定义数据。 

架构扩展示例：[使用架构扩展向组添加自定义数据](extensibility_schema_groups.md)


### <a name="schema-extensions-lifecycle"></a>架构扩展生命周期

当应用创建架构扩展定义时，系统会将该应用标记为该架构扩展的所有者。 

所有者应用可以在**状态**属性上使用 PATCH 操作将扩展转换为生命周期中的不同状态。基于当前状态，所有者应用可以更新或删除扩展。架构扩展的任何更新始终只能累加且不能间断。


| 状态 | 生命周期状态行为 |
|-------------|------------|
| InDevelopment | <ul><li>创建后的初始状态。所有者应用仍然在开发架构扩展。 </li><li>在此状态下，只有所有者应用可以使用此架构定义扩展资源实例，并且只能在注册所有者应用的同一目录进行。 </li><li>仅所有者应用可以使用增量更改来更新扩展定义或将其删除。 </li><li>所有者应用可以将扩展状态从**开发中**更改为**可用**。</li></ul> |
| 可用 | <ul><li>架构扩展可供任意租户中的所有应用使用。 </li><li>所有者应用将扩展设置为**可用**后，任何应用都只需将自定义数据添加到扩展中指定的资源类型的实例中（只要该应用具有该资源的相应权限）。创建新实例或更新现有实例时该应用可以分配自定义数据。 </li><li>仅所有者应用可以使用增量更改来更新扩展定义。 <br>- 在此状态下，任何应用都无法删除扩展定义。 </li><li>所有者应用可以将架构扩展状态从**可用**更改为**不推荐使用**。</li></ul> |
| 不推荐使用 | <ul><li>架构扩展定义不再可供读取或修改。 </li><li>任何应用都无法查看、更新、添加新属性或删除扩展。 </li><li>但是应用仍可读取、更新或删除现有扩展_属性值_。 </li><li>所有者应用可以将架构扩展从状态**不推荐使用**更改回**可用**。</li></ul> |

### <a name="supported-property-data-types"></a>受支持的属性数据类型

在架构扩展中定义属性时，支持以下数据类型：

| 属性类型 | 备注 |
|-------------|------------|
| Binary | 最多 256 字节。 |
| Boolean | 不支持消息、活动和帖子。 |
| 日期时间 | 必须以 ISO 8601 格式进行指定。存储为 UTC 格式。 |
| 整数 | 32 位值。不支持消息、活动和帖子。 |
| 字符串 | 最多 256 个字符。 |

>**注意：**不支持多值属性。

### <a name="azure-ad-directory-schema-extensions"></a>Azure AD 目录架构扩展

Azure AD 支持类似的扩展类型，在一些 [directoryObject](../api-reference/v1.0/resources/directoryObject.md) 资源中称其为[目录架构扩展](https://msdn.microsoft.com/en-us/library/azure/ad/graph/howto/azure-ad-graph-api-directory-schema-extensions)。虽然必须使用 Azure AD Graph API 创建并管理目录架构扩展的定义，但是可以使用 Microsoft Graph API 添加、获取、更新和删除这些扩展的属性中的数据。

## <a name="permissions"></a>权限

还需要对特定资源执行读取或写入操作所需的相同[权限](./permissions_reference.md)，以便对该资源上的任意扩展数据执行读取或写入操作。例如，对于能够使用自定义应用数据更新登录用户的个人资料的应用，必须向该应用授予 * User.ReadWrite.All * 权限。

此外，要创建和管理架构扩展定义，必须向应用程序授予 *Directory.AccessAsUser.All* 权限。

## <a name="data-limits"></a>数据限制

### <a name="open-extension-limits"></a>开放扩展限制
以下限制适用于目录资源（如**用户**、**组**、**设备**）：

- 每个开放扩展最多可以包含 2KB 的数据（包括扩展定义本身）。
- 应用程序最多可为每个资源实例添加两个开放扩展。

### <a name="schema-extension-limits"></a>架构扩展限制
应用程序最多可以创建五个**架构扩展**定义。

## <a name="known-limitations"></a>已知限制

有关使用扩展的已知限制，请参阅已知问题文章中的[扩展部分](known_issues.md#extensions)。

## <a name="extension-examples"></a>扩展示例

[使用开放扩展向用户添加自定义数据](extensibility_open_users.md)

[使用架构扩展向组添加自定义数据](extensibility_schema_groups.md)

## <a name="see-also"></a>另请参阅

[Office 365 域](https://technet.microsoft.com/en-us/library/office-365-domains.aspx)

[添加并验证 Office 365 租户的域](http://office365support.ca/adding-and-verifying-a-domain-for-the-new-office-365/)
